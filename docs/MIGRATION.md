# Migration Guide: clicksend-client v5 (legacy) → clicksend-client v6 (v2)

This guide helps you migrate from the legacy ClickSend Python SDK (`pip install clicksend-client`, `import clicksend_client`) to the current v2 SDK (`pip install --upgrade clicksend-client`, `import clicksend`). The two SDKs are **not drop-in compatible** — the import name, method names, request/response shapes, the exception module, and a few internals have all changed. Read this guide fully before upgrading, then use the class/method mapping tables to update your code.

## Contents

1. [Why this migration isn't a drop-in replacement](#1-why-this-migration-isnt-a-drop-in-replacement)
2. [Installation & imports](#2-installation--imports)
3. [Authentication & client setup](#3-authentication--client-setup)
4. [Base path / URL changes](#4-base-path--url-changes)
5. [Method naming convention change](#5-method-naming-convention-change)
6. [Request payloads: `*Request` models replace reusable domain models](#6-request-payloads-request-models-replace-reusable-domain-models)
7. [Response payloads are now properly typed](#7-response-payloads-are-now-properly-typed)
8. [Error handling changes](#8-error-handling-changes)
9. [Removed: `async_req` threading — plus new per-call request controls](#9-removed-async_req-threading--plus-new-per-call-request-controls)
10. [Class-by-class mapping (all 37 legacy classes)](#10-class-by-class-mapping-all-37-legacy-classes)
11. [Side-by-side examples for common operations](#11-side-by-side-examples-for-common-operations)
12. [The Voice naming trap (read this before touching voice code)](#12-the-voice-naming-trap-read-this-before-touching-voice-code)
13. [Endpoints/methods removed in v2](#13-endpointsmethods-removed-in-v2)
14. [Brand-new resources and methods in v2](#14-brand-new-resources-and-methods-in-v2)
15. [Step-by-step migration checklist](#15-step-by-step-migration-checklist)

## 1. Why this migration isn't a drop-in replacement

The legacy SDK grew organically against ClickSend's v3 API: one API class per rough "concept" (e.g. `EmailMarketingApi`, `TransactionalEmailApi`, `MasterEmailTemplatesApi`, `UserEmailTemplatesApi`, `EmailDeliveryReceiptRulesApi` were five *separate* classes), method names followed a `resource_path` + HTTP verb pattern (`sms_send_post`, `sms_history_get`), request bodies were broad reusable domain models (`SmsMessage`, `SmsMessageCollection`), and every response body was typed `str` and never deserialized.

The v2 SDK is generated fresh from ClickSend's current OpenAPI v3 specification, which:

- Groups methods into **one class per resource/tag** (26 classes instead of 37 — several legacy classes were merged, one was split, and the Fax, Letters, and Postcards classes were dropped entirely — see [§13](#13-endpointsmethods-removed-in-v2)).
- Names methods after the endpoint's **operationId** (`send_sms`, `view_sms_history`, `export_sms_history`) instead of `resource` + verb.
- Wraps every request body in a dedicated, single-purpose `*Request` model instead of reusing broad domain models.
- Uses **`pydantic` v2 models** for every request and response — full validation, real types, IDE autocomplete. Responses are deserialized into a specific per-operation model class.
- Moves the public exception to `clicksend.rest.ApiException` and adds status-specific subclasses (`BadRequestException`, `NotFoundException`, …).
- Drops Python 2 support (no more `six`), drops the bundled `certifi`, requires **Python 3.10+** (`pyproject.toml` lists `>=3.9`, but `setup.py` and the README both require `3.10`), and adds `pydantic` / `typing-extensions`.
- Drops the `async_req` thread-pool execution model — calls are synchronous only (see [§9](#9-removed-async_req-threading--plus-new-per-call-request-controls)).

None of this changes the underlying REST API — it's the same ClickSend v3 API — but it does change **every call site** in your existing integration.

## 2. Installation & imports

| | Legacy | v2 |
|---|---|---|
| Distribution name | `clicksend-client` | `clicksend-client` (unchanged) |
| Version at time of writing | `5.0.91` | `6.0.2` |
| **Import name** | `import clicksend_client` | `import clicksend` |
| Python supported | 2.7 and 3.4+ | **3.10+** |
| Runtime deps | `certifi`, `python-dateutil`, `six`, `urllib3>=1.23` | `urllib3>=2.1,<3`, `python-dateutil>=2.8.2`, `pydantic>=2.11`, `typing-extensions>=4.7.1` |
| Response validation | none (`str`) | `pydantic` v2 models |

```bash
# Upgrade in place — v2 is the next major version of the same package
pip install --upgrade clicksend-client
```

> v2 publishes under the **same distribution name** as the legacy SDK (`clicksend-client`), as a new major version (6.x). Upgrading replaces the legacy package, so the two can't be installed side by side. If your `requirements.txt` pins `clicksend-client<6` (or `==5.x`), bump it to `>=6,<7`. The **import name** does change (`clicksend_client` → `clicksend`), so existing imports fail loudly after the upgrade until you update them.

Every symbol you used to import from `clicksend_client` now comes from `clicksend`:

```python
# Legacy
from clicksend_client import SMSApi, ApiClient, Configuration
from clicksend_client.rest import ApiException

# v2
from clicksend import SmsApi, ApiClient, Configuration
from clicksend.rest import ApiException
```

The difference is *which* classes exist and what they're named (see [§10](#10-class-by-class-mapping-all-37-legacy-classes) below). Both SDKs re-export their API and model classes off the package root, so `from clicksend import <Name>` plus editor autocomplete is often the fastest way to discover a renamed method or model.

## 3. Authentication & client setup

The building blocks are the same three objects — `Configuration`, `ApiClient`, an `*Api` class — but how you wire them differs.

```python
# Legacy — Configuration() takes NO constructor args; set attributes after construction
import clicksend_client
from clicksend_client.rest import ApiException

configuration = clicksend_client.Configuration()
configuration.username = 'YOUR_USERNAME'
configuration.password = 'YOUR_API_KEY'

api_instance = clicksend_client.SMSApi(clicksend_client.ApiClient(configuration))
```

```python
# v2 — Configuration() accepts keyword args; ApiClient is a context manager
import os
import clicksend
from clicksend.rest import ApiException

configuration = clicksend.Configuration(
    username=os.environ["CLICKSEND_USERNAME"],
    password=os.environ["CLICKSEND_API_KEY"],
)

with clicksend.ApiClient(configuration) as api_client:
    sms_api = clicksend.SmsApi(api_client)
```

What changed:

| | Legacy | v2 |
|---|---|---|
| `Configuration()` constructor | no args; set `.username` / `.password` afterwards | accepts `username=`, `password=`, `host=`, `retries=`, … as kwargs (attribute-setting still works too) |
| `ApiClient` lifecycle | plain object | supports `with clicksend.ApiClient(configuration) as api_client:` (recommended — closes the connection pool) |
| Basic-auth key in `configuration.auth_settings()` | `'BasicAuth'` (capital B) | `'basicAuth'` (lowercase b) |
| Default `User-Agent` | generic Swagger-Codegen UA | `ClickSend-SDK/6.0.2/python`, settable via `api_client.user_agent = "..."` |

If your code reads or mutates `configuration.auth_settings()['BasicAuth']` directly (uncommon), update the key to `'basicAuth'`. If you only ever set `.username` / `.password`, **no change is needed** there beyond the import rename.

## 4. Base path / URL changes

| | Legacy | v2 |
|---|---|---|
| Default host | `https://rest.clicksend.com/v3` | `https://rest.clicksend.com` |
| Per-method path | `/sms/send` (no version prefix — it's baked into the host) | `/v3/sms/send` (the `/v3` prefix is part of each method's path) |
| Override attribute | `configuration.host` | `configuration.host` (same name) |

The final resolved URL is identical in both cases (`https://rest.clicksend.com/v3/sms/send`). This only matters if:

- You've overridden `configuration.host` (e.g. to point at a proxy or a mock server). If your custom host currently ends in `/v3` for the legacy SDK, **remove the `/v3` suffix** when you switch to v2 — otherwise you'll request `.../v3/v3/sms/send`.
- You construct raw URLs anywhere in test mocks/fixtures that assume the legacy host.

## 5. Method naming convention change

Every method on every API class has been renamed. There is no shared prefix/suffix rule you can find-and-replace — the new names follow each endpoint's `operationId` (snake_cased), which reads like an English phrase, while the old ones followed `resource_path` + HTTP verb.

| Legacy | v2 |
|---|---|
| `sms_send_post` | `send_sms` |
| `sms_history_get` | `view_sms_history` |
| `sms_history_export_get` | `export_sms_history` |
| `sms_templates_by_template_id_delete` | `delete_sms_template` |
| `lists_contacts_by_list_id_post` | `create_new_contact` |
| `subaccounts_post` | `create_subaccount` |
| `voice_lang_get` | `view_voice_languages` |
| `numbers_search_by_country_get` | `view_available_numbers` |

**You cannot mechanically derive the new name from the old one.** Use the mapping tables in [§10](#10-class-by-class-mapping-all-37-legacy-classes)–[§11](#11-side-by-side-examples-for-common-operations), or import the relevant `*Api` class and use your editor's autocomplete — the new names are descriptive enough that the right method is usually the first sensible match.

## 6. Request payloads: `*Request` models replace reusable domain models

Legacy methods took a broad, reusable domain model directly as the payload:

```python
# Legacy
from clicksend_client import SmsMessage, SmsMessageCollection

sms_message = SmsMessage(
    to='+61411111111',
    body='Hello from ClickSend!',
    source='php',
)
collection = SmsMessageCollection(messages=[sms_message])

sms_api.sms_send_post(collection)
```

v2 introduces **one dedicated `*Request` model per operation**, and every method also takes a leading optional `content_type` parameter for the `Content-Type` header:

```python
# v2
from clicksend import SendSmsRequest

request = SendSmsRequest(
    messages=[
        {"to": "+61411111111", "body": "Hello from ClickSend!", "source": "sdk"}
    ]
)

sms_api.send_sms(send_sms_request=request)
# a plain dict works too — pydantic coerces it:
sms_api.send_sms(send_sms_request={"messages": [{"to": "+61411111111", "body": "Hi"}]})
```

Practical implications:

- **The old domain-model class names mostly don't exist in v2.** `SmsMessage`, `SmsMessageCollection`, `Email`, `Voice`, `Contact`, `ContactList`, `Subaccount`, etc. are gone. The `models/` folder went from 47 files to 383, almost all named after a specific operation (`send_sms_request.py`, `create_new_contact_request.py`, `create_subaccount_request.py`, …) rather than a domain noun. Nested list items get their own generated models too (e.g. `SendSmsRequestMessagesInner`).
- **Pass the payload as a keyword argument.** v2 signatures are `method(content_type=None, <name>_request=None, ...)` with everything optional. `sms_api.send_sms(send_sms_request=...)` is the safe form. If you port a legacy positional call verbatim — `sms_api.send_sms(collection)` — `collection` lands in `content_type` and the request body is empty. Always name the payload arg.
- **`content_type`** is optional and effectively always `application/json`; you can omit it. It exists positionally in every method, which is the main reason not to call these methods positionally.
- **Field names are snake_case**, validated and serialized by `pydantic` via field aliases. The one field that needs attention is the SMS/MMS/email **sender**: legacy exposed it as the Python attribute `_from` (JSON `from`); in v2 the model attribute is `var_from` with `alias="from"`. Build it with `{"from": "sdk"}` in a dict, or `var_from="sdk"` via the model constructor.
- `source` now defaults to `sdk-python` on SMS, MMS, and voice message items if you don't set it (legacy had no default).

## 7. Response payloads are now properly typed

Legacy responses were **always typed `str`** and never deserialized — you parsed `response` yourself with `json.loads` and dug through dicts, knowing the shape out-of-band from the API docs.

```python
# Legacy — return value is a raw JSON string
response = sms_api.sms_send_post(collection)
import json
data = json.loads(response)["data"]        # manual, untyped
```

v2 deserializes every response into a specific per-operation `pydantic` model (e.g. `SendSms`, `ViewSmsHistory`, `CalculateSmsPrice`), so the return value is typed and autocomplete-friendly:

```python
# v2 — return value is a SendSms instance
response = sms_api.send_sms(send_sms_request=request)
print(response.data)                       # typed attribute access
print(response.to_dict())                  # or a plain dict
print(response.to_json())                  # or a JSON string
```

If your legacy code does `json.loads(response)` or manual property digging, you can delete that logic — the SDK does it now. Audit any code that assumed the return value was a `str`.

To get the status code and headers alongside the body, use the `*_with_http_info` variant of any method (it returns an `ApiResponse` with `.data`, `.status_code`, `.headers`); a `*_without_preload_content` variant returns the raw `urllib3` response for streaming.

## 8. Error handling changes

Both SDKs raise `ApiException` on non-2xx responses, and its core attributes are unchanged — but the **import path moved** and v2 adds **status-specific subclasses**.

| | Legacy | v2 |
|---|---|---|
| Import | `from clicksend_client.rest import ApiException` | `from clicksend.rest import ApiException` (also `from clicksend import ApiException`) |
| Base class | `Exception` | `clicksend.exceptions.OpenApiException` → `Exception` |
| Attributes | `.status`, `.reason`, `.body`, `.headers` | `.status`, `.reason`, `.body`, `.headers`, **`.data`** (deserialized error model when available) |
| Subclasses | none | `BadRequestException` (400), `UnauthorizedException` (401), `ForbiddenException` (403), `NotFoundException` (404), `ConflictException` (409), `UnprocessableEntityException` (422), `ServiceException` (5xx) |

```python
# Legacy
from clicksend_client.rest import ApiException

try:
    sms_api.sms_send_post(collection)
except ApiException as e:
    print(e.status, e.body)

# v2 — catch the base class, or a specific subclass
from clicksend.rest import ApiException
from clicksend.exceptions import UnauthorizedException

try:
    sms_api.send_sms(send_sms_request=request)
except UnauthorizedException:
    refresh_credentials()
except ApiException as e:
    print(e.status)    # e.g. 400
    print(e.body)      # raw response body
    print(e.data)      # deserialized error model, when the SDK could parse one
```

**Audit every `except ApiException` block.** Fix the import, and note that `except clicksend_client.rest.ApiException` will no longer catch anything from v2. Client-side validation failures now raise `pydantic.ValidationError` (or `clicksend.exceptions.ApiTypeError` / `ApiValueError`) *before* the HTTP call — handle those where you build requests from untrusted input.

## 9. Removed: `async_req` threading — plus new per-call request controls

**Removed.** The legacy SDK ran every method synchronously by default but accepted `async_req=True` to dispatch the call on a `multiprocessing.pool.ThreadPool` and return a result handle:

```python
# Legacy — no longer supported
thread = sms_api.sms_send_post(collection, async_req=True)
result = thread.get()
```

v2 has **no `async_req`, no thread pool, and no `asyncio` client** — calls are synchronous. If you relied on `async_req` for concurrency, wrap calls in your own `concurrent.futures.ThreadPoolExecutor`, and give each worker its own `ApiClient`.

**New.** Every v2 method accepts a set of underscore-prefixed keyword controls for per-call customization — the nearest equivalent to a request hook:

| Parameter | Purpose |
|---|---|
| `_headers={"X-Request-Id": "..."}` | extra headers for this one call |
| `_request_timeout=5.0` or `(connect, read)` | per-call timeout override |
| `_request_auth={...}` | override auth for this one call |
| `_host_index=0` | pick an alternate server when the spec defines several |

Client-wide options moved onto `Configuration`: `Configuration(retries=urllib3.util.Retry(...))` for automatic retries, and `api_client.user_agent = "..."` to change the `User-Agent` (`ClickSend-SDK/6.0.2/python` by default).

## 10. Class-by-class mapping (all 37 legacy classes)

26 v2 classes now cover what used to be 37 legacy classes. Some legacy classes merged (five email classes → one `EmailApi`); the Fax, Letters, and Postcards classes were **dropped entirely** (see [§13](#13-endpointsmethods-removed-in-v2)); and — critically — the two Voice classes **swapped roles** in v2 naming (see [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code)).

| Legacy class | → | New class(es) | Notes |
|---|---|---|---|
| `AccountApi` | → | `ManagementApi`, `VerificationApi` | Split: `account_get`/`account_useage_by_subaccount_get` → `ManagementApi`; `forgot_password_put`/`forgot_username_put` → `VerificationApi`. Four methods have no v2 equivalent — see [§13](#13-endpointsmethods-removed-in-v2). |
| `AccountRechargeApi` | → | `TransactionsApi` | Renamed 1:1 (6 methods). |
| `ContactApi` | → | `ContactsApi`, `ListsApi` | Split: single-contact-by-id CRUD → `ContactsApi`; list-scoped contact ops (create/list/copy/transfer/remove-opted-out) → `ListsApi`. |
| `ContactListApi` | → | `ListsApi` | Merged into `ListsApi`. |
| `CountriesApi` | → | `InternationalMessagingApi` | `countries_get` → `list_countries`. |
| `DeliveryIssuesApi` | → | `MessageDeliveryApi` | Renamed. Unrelated to the delivery-*receipt-rule* classes despite the similar name. |
| `DetectAddressApi` | → | _(removed)_ | Address detection/parsing has no v2 equivalent — see [§13](#13-endpointsmethods-removed-in-v2). |
| `EmailDeliveryReceiptRulesApi` | → | `EmailApi` | Folded into the unified `EmailApi`. |
| `EmailMarketingApi` | → | `EmailApi` | Folded into the unified `EmailApi`. |
| `EmailToSmsApi` | → | `EmailToSmsApi` | Same class name, methods renamed (7 → 7). |
| `FAXApi` | → | _(removed)_ | Fax is not part of the v2 SDK — see [§13](#13-endpointsmethods-removed-in-v2). |
| `FAXDeliveryReceiptRulesApi` | → | _(removed)_ | Fax is not part of the v2 SDK — see [§13](#13-endpointsmethods-removed-in-v2). |
| `GlobalSendingApi` | → | `InternationalMessagingApi` | Folded in (`user_countries_*` → `view_countries` / `select_countries_for_global_sending` / `agree_to_rules_and_regulation`; `list_countries_get` → `get_countries_for_global_sending`). |
| `InboundFAXRulesApi` | → | _(removed)_ | Fax is not part of the v2 SDK — see [§13](#13-endpointsmethods-removed-in-v2). |
| `InboundSMSRulesApi` | → | `SmsApi` | Folded in as `*_sms_inbound_automation(s)`. |
| `MMSApi` | → | `MmsApi` | Renamed 1:1 for 4 methods; 2 dropped — see [§13](#13-endpointsmethods-removed-in-v2). |
| `MasterEmailTemplatesApi` | → | `EmailApi` | Folded into the unified `EmailApi`. |
| `MmsCampaignApi` | → | `MmsCampaignsApi` | Renamed 1:1 (6 methods). |
| `NumberApi` | → | `NumbersApi` | Renamed 1:1 (3 methods), plus a brand-new `register_numbers` — see [§14](#14-brand-new-resources-and-methods-in-v2). |
| `PostLetterApi` | → | _(removed)_ | Letters is not part of the v2 SDK — see [§13](#13-endpointsmethods-removed-in-v2). |
| `PostPostcardApi` | → | _(removed)_ | Postcards is not part of the v2 SDK — see [§13](#13-endpointsmethods-removed-in-v2). |
| `PostReturnAddressApi` | → | `AddressesApi` | Renamed (5 methods): `post_return_addresses_*` → `*_return_address(es)`. |
| `ReferralAccountApi` | → | `ReferralsApi` | `referral_accounts_get` → `view_referral_accounts`. |
| `ResellerAccountApi` | → | `ResellerApi` | Merged with `TransferCreditApi`. |
| `SMSApi` | → | `SmsApi` | Renamed 1:1 for all core methods. |
| `SMSDeliveryReceiptRulesApi` | → | `SmsApi` | Folded in as `*_sms_delivery_receipt_rule(s)`. |
| `SearchApi` | → | `ListsApi` | `search_contacts_lists_get` → `view_contact_lists`. |
| `SmsCampaignApi` | → | `SmsCampaignsApi` | Renamed 1:1 (6 methods). |
| `StatisticsApi` | → | `StatisticsApi` | Same class name: `statistics_sms_get` → `view_sms_statistics`, `statistics_voice_get` → `view_voice_statistics`. |
| `SubaccountApi` | → | `SubaccountsApi` | Renamed 1:1 (6 methods). |
| `TimezonesApi` | → | `InternationalMessagingApi` | `timezones_get` → `timezones`. |
| `TransactionalEmailApi` | → | `EmailApi` | Folded into the unified `EmailApi`. |
| `TransferCreditApi` | → | `ResellerApi` | Merged with `ResellerAccountApi`; `reseller_transfer_credit_put` → `reseller_transfer_credit`. |
| `UploadApi` | → | `UploadsApi` | `uploads_post` → `upload_a_media_file`. |
| `UserEmailTemplatesApi` | → | `EmailApi` | Folded into the unified `EmailApi`. |
| `VoiceApi` (send/history/price/lang) | → | **`VoiceMessagingApi`** | ⚠️ See [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) — this is *not* the new `VoiceApi`. 2 methods dropped — see [§13](#13-endpointsmethods-removed-in-v2). |
| `VoiceDeliveryReceiptRulesApi` | → | **`VoiceApi`** | ⚠️ See [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) — the new `VoiceApi` only has delivery-receipt-rule methods. |

`AlphaTagsApi`, `DefaultSendersApi`, `OwnNumbersApi`, and `UrlShorteningApi` in v2 have **no legacy predecessor at all** — see [§14](#14-brand-new-resources-and-methods-in-v2).

### Email: the five legacy classes → `EmailApi`

| Legacy | v2 (`EmailApi`) |
|---|---|
| `TransactionalEmailApi.email_send_post` | `send_email` |
| `TransactionalEmailApi.email_history_get` | `view_email_history` |
| `TransactionalEmailApi.email_history_export_get` | `export_email_history` |
| `TransactionalEmailApi.email_price_post` | `calculate_email_price` |
| `EmailMarketingApi.email_campaign_post` | `send_email_campaign` |
| `EmailMarketingApi.email_campaigns_get` | `view_all_email_campaigns` |
| `EmailMarketingApi.email_campaign_get` | `view_email_campaign` |
| `EmailMarketingApi.email_campaign_put` | `update_email_campaign` |
| `EmailMarketingApi.cancel_email_campaign_put` | `cancel_email_campaign` |
| `EmailMarketingApi.email_campaign_price_post` | `calculate_email_campaign_price` |
| `EmailMarketingApi.email_campaign_history_get` | `view_email_campaign_history` |
| `EmailMarketingApi.email_campaign_history_export_get` | `export_email_campaign_history` |
| `EmailMarketingApi.allowed_email_address_get` | `view_allowed_email_addresses` |
| `EmailMarketingApi.allowed_email_address_post` | `create_allowed_email_address` |
| `EmailMarketingApi.specific_allowed_email_address_get` | `view_allowed_email_address` |
| `EmailMarketingApi.specific_allowed_email_address_delete` | `delete_allowed_email_address` |
| `EmailMarketingApi.verify_allowed_email_address_get` | `verify_allowed_email_address` |
| `EmailMarketingApi.send_verification_token_get` | `send_email_verification_token` |
| `UserEmailTemplatesApi.email_templates_get` | `view_email_templates` |
| `UserEmailTemplatesApi.email_template_get` | `view_email_template` |
| `UserEmailTemplatesApi.email_template_post` | `create_email_template` |
| `UserEmailTemplatesApi.email_template_put` | `update_email_template` |
| `UserEmailTemplatesApi.email_template_delete` | `delete_email_template` |
| `MasterEmailTemplatesApi.master_email_templates_get` | `view_master_email_templates` |
| `MasterEmailTemplatesApi.master_email_template_get` | `view_master_email_template` |
| `MasterEmailTemplatesApi.master_email_template_categories_get` | `view_template_categories` |
| `MasterEmailTemplatesApi.master_email_template_category_get` | `view_template_category` |
| `MasterEmailTemplatesApi.master_email_templates_in_category_get` | `view_templates_in_category` |
| `EmailDeliveryReceiptRulesApi.email_delivery_receipt_automations_get` | `view_email_delivery_receipt_rules` |
| `EmailDeliveryReceiptRulesApi.email_delivery_receipt_automation_get` | `view_email_delivery_receipt_rule` |
| `EmailDeliveryReceiptRulesApi.email_delivery_receipt_automation_post` | `create_email_delivery_receipt_rule` |
| `EmailDeliveryReceiptRulesApi.email_delivery_receipt_automation_put` | `update_email_delivery_receipt_rule` |
| `EmailDeliveryReceiptRulesApi.email_delivery_receipt_automation_delete` | `delete_email_delivery_receipt_rule` |

> `EmailMarketingApi.email_campaign_put` in the legacy SDK reused an `EmailCampaign` model for update; v2's `update_email_campaign` takes an `UpdateEmailCampaignRequest`. Same story for every other method above.

### SMS: `SMSApi` + `InboundSMSRulesApi` + `SMSDeliveryReceiptRulesApi` → `SmsApi`

| Legacy | v2 (`SmsApi`) |
|---|---|
| `SMSApi.sms_send_post` | `send_sms` |
| `SMSApi.sms_history_get` | `view_sms_history` |
| `SMSApi.sms_history_export_get` | `export_sms_history` |
| `SMSApi.sms_price_post` | `calculate_sms_price` |
| `SMSApi.sms_cancel_all_put` | `cancel_all_sms` |
| `SMSApi.sms_cancel_by_message_id_put` | `cancel_sms` |
| `SMSApi.sms_inbound_get` | `view_inbound_sms` |
| `SMSApi.sms_inbound_post` | `create_test_inbound_sms` |
| `SMSApi.sms_inbound_read_put` | `mark_inbound_sms_as_read` |
| `SMSApi.sms_inbound_read_by_message_id_put` | `mark_specific_inbound_sms_message_as_read` |
| `SMSApi.sms_receipts_get` | `view_sms_receipts` |
| `SMSApi.sms_receipts_by_message_id_get` | `view_specific_sms_receipt` |
| `SMSApi.sms_receipts_post` | `create_test_sms_receipt` |
| `SMSApi.sms_receipts_read_put` | `mark_sms_receipt_as_read` |
| `SMSApi.sms_templates_get` | `view_sms_templates` |
| `SMSApi.sms_templates_post` | `create_sms_template` |
| `SMSApi.sms_templates_by_template_id_put` | `update_sms_template` |
| `SMSApi.sms_templates_by_template_id_delete` | `delete_sms_template` |
| `InboundSMSRulesApi.sms_inbound_automations_get` | `view_sms_inbound_automations` |
| `InboundSMSRulesApi.sms_inbound_automation_get` | `view_sms_inbound_automation` |
| `InboundSMSRulesApi.sms_inbound_automation_post` | `create_sms_inbound_automation` |
| `InboundSMSRulesApi.sms_inbound_automation_put` | `update_sms_inbound_automation` |
| `InboundSMSRulesApi.sms_inbound_automation_delete` | `delete_sms_inbound_automation` |
| `SMSDeliveryReceiptRulesApi.sms_delivery_receipt_automations_get` | `view_sms_delivery_receipt_rules` |
| `SMSDeliveryReceiptRulesApi.sms_delivery_receipt_automation_get` | `view_sms_delivery_receipt_rule` |
| `SMSDeliveryReceiptRulesApi.sms_delivery_receipt_automation_post` | `create_sms_delivery_receipt_rule` |
| `SMSDeliveryReceiptRulesApi.sms_delivery_receipt_automation_put` | `update_sms_delivery_receipt_rule` |
| `SMSDeliveryReceiptRulesApi.sms_delivery_receipt_automation_delete` | `delete_sms_delivery_receipt_rule` |
| — | `view_a_specific_sms_template` *(new — see [§14](#14-brand-new-resources-and-methods-in-v2))* |
| — | `view_a_specific_inbound_sms_message` *(new — see [§14](#14-brand-new-resources-and-methods-in-v2))* |

### Contacts & lists: `ContactApi` + `ContactListApi` + `SearchApi` → `ContactsApi` + `ListsApi`

| Legacy | v2 |
|---|---|
| `ContactApi.lists_contacts_by_list_id_and_contact_id_get` | `ContactsApi.get_specific_contact` |
| `ContactApi.lists_contacts_by_list_id_and_contact_id_put` | `ContactsApi.update_contact` |
| `ContactApi.lists_contacts_by_list_id_and_contact_id_delete` | `ContactsApi.delete_contact` |
| `ContactApi.lists_contacts_by_list_id_post` | `ListsApi.create_new_contact` |
| `ContactApi.lists_contacts_by_list_id_get` | `ListsApi.view_list_contacts` |
| `ContactApi.lists_copy_contact_put` | `ListsApi.copy_contact_to_list` |
| `ContactApi.lists_transfer_contact_put` | `ListsApi.transfer_contact_to_list` |
| `ContactApi.lists_remove_opted_out_contacts_by_list_id_and_opt_out_list_id_put` | `ListsApi.remove_opted_out_contacts` |
| `ContactListApi.lists_get` | `ListsApi.view_lists` |
| `ContactListApi.lists_post` | `ListsApi.create_list` |
| `ContactListApi.lists_by_list_id_get` | `ListsApi.view_specific_list` |
| `ContactListApi.lists_by_list_id_put` | `ListsApi.update_list` |
| `ContactListApi.lists_by_list_id_delete` | `ListsApi.delete_list` |
| `ContactListApi.lists_import_by_list_id_post` | `ListsApi.import_contacts` |
| `ContactListApi.lists_remove_duplicates_by_list_id_put` | `ListsApi.remove_duplicate_contacts` |
| `SearchApi.search_contacts_lists_get` | `ListsApi.view_contact_lists` |

### Account & billing

| Legacy | v2 |
|---|---|
| `AccountApi.account_get` | `ManagementApi.view_account_details` |
| `AccountApi.account_useage_by_subaccount_get` | `ManagementApi.view_account_usage` |
| `AccountApi.forgot_password_put` | `VerificationApi.forgot_password` |
| `AccountApi.forgot_username_put` | `VerificationApi.forgot_username` |
| `AccountRechargeApi.recharge_credit_card_get` | `TransactionsApi.current_payment_info` |
| `AccountRechargeApi.recharge_credit_card_put` | `TransactionsApi.update_payment_info` |
| `AccountRechargeApi.recharge_packages_get` | `TransactionsApi.view_recharge_packages` |
| `AccountRechargeApi.recharge_purchase_by_package_id_put` | `TransactionsApi.purchase_recharge_package` |
| `AccountRechargeApi.recharge_transactions_get` | `TransactionsApi.view_all_transactions` |
| `AccountRechargeApi.recharge_transactions_by_transaction_id_get` | `TransactionsApi.view_specific_transaction` |
| `ResellerAccountApi.reseller_accounts_get` | `ResellerApi.view_client_accounts` |
| `ResellerAccountApi.reseller_accounts_post` | `ResellerApi.create_reseller_account` |
| `ResellerAccountApi.reseller_accounts_by_client_user_id_get` | `ResellerApi.view_specific_client_account` |
| `ResellerAccountApi.reseller_accounts_by_client_user_id_put` | `ResellerApi.update_client_account` |
| `TransferCreditApi.reseller_transfer_credit_put` | `ResellerApi.reseller_transfer_credit` |
| `SubaccountApi.subaccounts_get` | `SubaccountsApi.view_subaccounts` |
| `SubaccountApi.subaccounts_post` | `SubaccountsApi.create_subaccount` |
| `SubaccountApi.subaccounts_by_subaccount_id_get` | `SubaccountsApi.view_specific_subaccount` |
| `SubaccountApi.subaccounts_by_subaccount_id_put` | `SubaccountsApi.update_subaccount` |
| `SubaccountApi.subaccounts_by_subaccount_id_delete` | `SubaccountsApi.delete_subaccount` |
| `SubaccountApi.subaccounts_regen_api_key_by_subaccount_id_put` | `SubaccountsApi.generate_new_api_key` |
| `ReferralAccountApi.referral_accounts_get` | `ReferralsApi.view_referral_accounts` |

### Numbers, addresses, uploads, international, delivery issues

| Legacy | v2 |
|---|---|
| `NumberApi.numbers_get` | `NumbersApi.view_your_numbers` |
| `NumberApi.numbers_search_by_country_get` | `NumbersApi.view_available_numbers` |
| `NumberApi.numbers_buy_by_dedicated_number_post` | `NumbersApi.purchase_dedicated_number` |
| `PostReturnAddressApi.post_return_addresses_get` | `AddressesApi.view_your_return_addresses` |
| `PostReturnAddressApi.post_return_addresses_post` | `AddressesApi.create_return_address` |
| `PostReturnAddressApi.post_return_addresses_by_return_address_id_get` | `AddressesApi.view_specific_return_address` |
| `PostReturnAddressApi.post_return_addresses_by_return_address_id_put` | `AddressesApi.update_return_address` |
| `PostReturnAddressApi.post_return_addresses_by_return_address_id_delete` | `AddressesApi.delete_return_address` |
| `UploadApi.uploads_post` | `UploadsApi.upload_a_media_file` |
| `CountriesApi.countries_get` | `InternationalMessagingApi.list_countries` |
| `TimezonesApi.timezones_get` | `InternationalMessagingApi.timezones` |
| `GlobalSendingApi.list_countries_get` | `InternationalMessagingApi.get_countries_for_global_sending` |
| `GlobalSendingApi.user_countries_get` | `InternationalMessagingApi.view_countries` |
| `GlobalSendingApi.user_countries_post` | `InternationalMessagingApi.select_countries_for_global_sending` |
| `GlobalSendingApi.user_countries_agree_post` | `InternationalMessagingApi.agree_to_rules_and_regulation` |
| `DeliveryIssuesApi.delivery_issues_get` | `MessageDeliveryApi.get_all_delivery_issues` |
| `DeliveryIssuesApi.delivery_issues_post` | `MessageDeliveryApi.create_delivery_issue` |

### MMS, campaigns, voice, statistics

| Legacy | v2 |
|---|---|
| `MMSApi.mms_send_post` | `MmsApi.send_mms` |
| `MMSApi.mms_history_get` | `MmsApi.view_mms_history` |
| `MMSApi.mms_history_export_get` | `MmsApi.export_mms_history` |
| `MMSApi.mms_price_post` | `MmsApi.calculate_mms_price` |
| `MmsCampaignApi.mms_campaigns_send_post` | `MmsCampaignsApi.send_mms_campaign` |
| `MmsCampaignApi.mms_campaigns_get` | `MmsCampaignsApi.view_all_mms_campaigns` |
| `MmsCampaignApi.mms_campaign_by_mms_campaign_id_get` | `MmsCampaignsApi.view_mms_campaign` |
| `MmsCampaignApi.mms_campaigns_by_mms_campaign_id_put` | `MmsCampaignsApi.update_mms_campaign` |
| `MmsCampaignApi.mms_campaigns_cancel_by_mms_campaign_id_put` | `MmsCampaignsApi.cancel_mms_campaign` |
| `MmsCampaignApi.mms_campaigns_price_post` | `MmsCampaignsApi.calculate_mms_campaign_price` |
| `SmsCampaignApi.sms_campaigns_send_post` | `SmsCampaignsApi.send_sms_campaign` |
| `SmsCampaignApi.sms_campaigns_get` | `SmsCampaignsApi.view_sms_campaigns` |
| `SmsCampaignApi.sms_campaign_by_sms_campaign_id_get` | `SmsCampaignsApi.view_specific_sms_campaign` |
| `SmsCampaignApi.sms_campaigns_by_sms_campaign_id_put` | `SmsCampaignsApi.update_sms_campaign` |
| `SmsCampaignApi.sms_campaigns_cancel_by_sms_campaign_id_put` | `SmsCampaignsApi.cancel_sms_campaign` |
| `SmsCampaignApi.sms_campaigns_price_post` | `SmsCampaignsApi.calculate_sms_campaign_price` |
| `VoiceApi.voice_send_post` | `VoiceMessagingApi.send_voice_message` ⚠️ [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) |
| `VoiceApi.voice_history_get` | `VoiceMessagingApi.get_voice_history` |
| `VoiceApi.voice_history_export_get` | `VoiceMessagingApi.export_voice_history` |
| `VoiceApi.voice_price_post` | `VoiceMessagingApi.calculate_voice_price` |
| `VoiceApi.voice_lang_get` | `VoiceMessagingApi.view_voice_languages` |
| `VoiceApi.voice_cancel_all_put` | `VoiceMessagingApi.cancel_all_voice_messages` |
| `VoiceApi.voice_cancel_by_message_id_put` | `VoiceMessagingApi.cancel_voice_message` |
| `VoiceApi.voice_receipts_get` | `VoiceMessagingApi.view_voice_receipts` |
| `VoiceDeliveryReceiptRulesApi.voice_delivery_receipt_automations_get` | `VoiceApi.view_voice_delivery_receipt_rules` ⚠️ [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) |
| `VoiceDeliveryReceiptRulesApi.voice_delivery_receipt_automation_get` | `VoiceApi.view_voice_delivery_receipt_rule` |
| `VoiceDeliveryReceiptRulesApi.voice_delivery_receipt_automation_post` | `VoiceApi.create_voice_delivery_receipt_rule` |
| `VoiceDeliveryReceiptRulesApi.voice_delivery_receipt_automation_put` | `VoiceApi.update_voice_delivery_receipt_rule` |
| `VoiceDeliveryReceiptRulesApi.voice_delivery_receipt_automation_delete` | `VoiceApi.delete_voice_delivery_receipt_rule` |
| `StatisticsApi.statistics_sms_get` | `StatisticsApi.view_sms_statistics` |
| `StatisticsApi.statistics_voice_get` | `StatisticsApi.view_voice_statistics` |

### Email-to-SMS: `EmailToSmsApi` → `EmailToSmsApi`

| Legacy | v2 |
|---|---|
| `sms_email_sms_get` | `view_allowed_emails` |
| `sms_email_sms_post` | `add_allowed_email` |
| `sms_email_sms_stripped_string_post` | `create_stripped_string_rule` |
| `sms_email_sms_stripped_string_get` | `view_stripped_string_rule` |
| `sms_email_sms_stripped_strings_get` | `view_stripped_string_rules` |
| `sms_email_sms_stripped_string_put` | `update_stripped_string_rule` |
| `sms_email_sms_stripped_string_delete` | `delete_stripped_string_rule` |

## 11. Side-by-side examples for common operations

### Send an SMS

```python
# Legacy
from clicksend_client import SmsMessage, SmsMessageCollection

msg = SmsMessage(to='+61411111111', body='Hello from ClickSend!', source='php')
collection = SmsMessageCollection(messages=[msg])

try:
    response = sms_api.sms_send_post(collection)
    print(response)                       # raw JSON string
except ApiException as e:
    print(e.status, e.body)

# v2
from clicksend import SendSmsRequest

request = SendSmsRequest(messages=[
    {"to": "+61411111111", "body": "Hello from ClickSend!", "source": "sdk"}
])

try:
    response = sms_api.send_sms(send_sms_request=request)
    print(response.data)                  # typed SendSms instance
except ApiException as e:
    print(e.status, e.body)
```

### View SMS history

```python
# Legacy — all params are optional keyword args
sms_api.sms_history_get(q=q, date_from=date_from, date_to=date_to, page=page, limit=limit)

# v2 — `page`/`limit`/`order_by` are still keyword args, but `order_by` is new
# and `limit` is validated to 15..100. Pass everything by name.
sms_api.view_sms_history(
    page=page, limit=limit, q=q, order_by="date:desc",
    date_from=date_from, date_to=date_to,
)
```

> Always pass these by keyword and check the current signature — parameter sets changed (this one gained `order_by`, and `limit` gained a 15-100 bound).

### Send an MMS / Email / Voice message

Same pattern on every channel — build a `Send<Channel>Request`, call `send_<channel>(...)`:

| Channel | Legacy call | v2 call |
|---|---|---|
| MMS | `mms_api.mms_send_post(mms_message_collection)` | `mms_api.send_mms(send_mms_request=send_mms_request)` |
| Email | `email_api.email_send_post(email)` | `email_api.send_email(send_email_request=send_email_request)` |
| Voice | `voice_api.voice_send_post(voice_collection)` (legacy `VoiceApi`) | `voice_messaging_api.send_voice_message(send_voice_message_request=req)` (⚠️ new `VoiceMessagingApi`, see [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code)) |

> **Fax, Letters, and Postcards are not part of the v2 SDK** — there is no `send_fax` / `post_letters_send` / `post_postcards_send` equivalent. See [§13](#13-endpointsmethods-removed-in-v2).

### Create a contact in a list

```python
# Legacy — contact model first, list_id (int) second
contact_api.lists_contacts_by_list_id_post(contact, list_id)

# v2 — list_id is now FIRST and a STRING; payload is a keyword arg
lists_api.create_new_contact(
    str(list_id),
    create_new_contact_request=create_new_contact_request,
)
```

### List contacts / lists — pagination parameters were dropped

```python
# Legacy — page / limit / updated_after were real keyword params
contact_api.lists_contacts_by_list_id_get(list_id, page=page, limit=limit, updated_after=ts)
contact_list_api.lists_get(page=page, limit=limit)
subaccount_api.subaccounts_get(page=page, limit=limit)

# v2 — those params no longer exist on the signature
lists_api.view_list_contacts(str(list_id))
lists_api.view_lists()
subaccounts_api.view_subaccounts()
```

**This is a real behavior change, not just a rename.** `ListsApi.view_lists`, `ListsApi.view_list_contacts`, and `SubaccountsApi.view_subaccounts` in v2 take no `page` / `limit` / `updated_after`. Verify against the current API reference how pagination is handled for any workflow that relied on them before you ship.

### Create a subaccount

```python
# Legacy
subaccount_api.subaccounts_post(subaccount)

# v2
subaccounts_api.create_subaccount(create_subaccount_request=create_subaccount_request)
```

## 12. The Voice naming trap (read this before touching voice code)

This is the single most confusing rename in the whole migration, and a naive search-and-replace of `VoiceApi` will silently point your code at the wrong class:

- Legacy **`VoiceApi`** (send a voice message, view/export history, calculate price, list voice languages, cancel, view receipts) → renamed to new **`VoiceMessagingApi`**.
- Legacy **`VoiceDeliveryReceiptRulesApi`** (create/update/delete/view delivery-receipt rules) → renamed to new **`VoiceApi`**.

The new `VoiceApi` has **nothing to do with sending voice calls** — it is purely the old delivery-receipt-rules class under a new name. To migrate voice-sending code, import `VoiceMessagingApi`:

```python
# Wrong — this runs, but VoiceApi in v2 only has delivery-receipt-rule methods
voice_api = clicksend.VoiceApi(api_client)
voice_api.send_voice_message(...)          # AttributeError

# Correct
voice_messaging_api = clicksend.VoiceMessagingApi(api_client)
voice_messaging_api.send_voice_message(send_voice_message_request=req)
```

## 13. Endpoints/methods removed in v2

### Entire products dropped

The **Fax**, **Letters**, and **Postcards** products have **no presence at all** in the v2 SDK — no API class, no models. If your integration sends faxes, letters, or postcards, there is currently no v2 SDK path for it; call the REST API directly or stay on the legacy SDK for those channels.

| Legacy class(es) | Covered (legacy) | v2 |
|---|---|---|
| `FAXApi`, `FAXDeliveryReceiptRulesApi`, `InboundFAXRulesApi` | send fax, fax history/export, fax price, fax receipts, fax delivery-receipt rules, inbound fax rules | _none_ |
| `PostLetterApi` | send letter, letter history/export, letter price | _none_ |
| `PostPostcardApi` | send postcard, postcard history/export, postcard price | _none_ |
| `DetectAddressApi` | address detection/parsing (`detect_address_post`) | _none_ |

### Individual methods dropped (class otherwise survived)

The following legacy operations have **no equivalent anywhere in the v2 SDK**. If your integration depends on any of these, check the current ClickSend API reference before upgrading — the underlying endpoint may have been retired, moved, or simply not covered by the new spec at build time:

- `AccountApi.account_post` — update account details
- `AccountApi.account_verify_send_put` — send account verification email
- `AccountApi.account_verify_verify_by_activation_token_put` — verify account by activation token
- `AccountApi.forgot_password_verify_put` — verify a forgotten-password token
- `MMSApi.mms_receipts_get` — view MMS delivery receipts
- `MMSApi.mms_receipts_read_put` — mark MMS receipts as read
- `VoiceApi.voice_receipts_post` (legacy class) — create a test voice receipt
- `VoiceApi.voice_receipts_read_put` (legacy class) — mark voice receipts as read

Additionally, **pagination parameters (`page`, `limit`, `updated_after`) were dropped** from several method signatures even where the class survived — notably `ListsApi.view_lists`, `ListsApi.view_list_contacts`, and `SubaccountsApi.view_subaccounts` (see [§11](#11-side-by-side-examples-for-common-operations)).

## 14. Brand-new resources and methods in v2

No legacy counterpart at all — nothing to migrate, but worth knowing they exist:

- **`AlphaTagsApi`** — `list_alpha_tags`, `get_alpha_tag`, `request_alpha_tag`, `delete_alpha_tag`
- **`DefaultSendersApi`** — `get_default_senders_list`, `get_default_sender_details`, `create_default_sender`, `update_default_sender`, `delete_default_sender`, `list_compliant_sender_types`
- **`OwnNumbersApi`** (Bring Your Own Number) — `list_own_numbers`, `get_own_number_detail`, `update_own_number`, `delete_own_number`, `request_own_number_verification_otp`, `verify_own_number_otp`
- **`UrlShorteningApi`** — `short_url_get_statistics`, `short_url_get_tracking`
- **`NumbersApi.register_numbers`** — number registration (alongside the renamed `NumberApi` methods)
- **`SmsApi.view_a_specific_inbound_sms_message`** and **`SmsApi.view_a_specific_sms_template`** — fetch a single inbound message / template by ID (legacy only exposed the list endpoints)

## 15. Step-by-step migration checklist

1. **Upgrade the dependency**: `pip install --upgrade clicksend-client` and bump any `<6` pin to `>=6,<7` ([§2](#2-installation--imports)).
2. **Rename the import**: `clicksend_client` → `clicksend` everywhere, including `clicksend_client.rest` → `clicksend.rest` for `ApiException`.
3. **Update client setup**: `Configuration(username=..., password=...)`, wrap usage in `with clicksend.ApiClient(configuration) as api_client:`, and rename API classes to their new casing (`SMSApi` → `SmsApi`, `MMSApi` → `MmsApi`, …). **Pay special attention to `VoiceApi` → `VoiceMessagingApi`** ([§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code)).
4. **Rebuild every request payload** with the matching `*Request` model (or a plain dict) instead of the old domain model, and pass it as a **keyword argument** (`send_sms_request=...`) so it doesn't land in the leading `content_type` slot ([§6](#6-request-payloads-request-models-replace-reusable-domain-models)). Watch the sender field: `_from` → `var_from` / `{"from": ...}`.
5. **Rename every method call** using the [§10](#10-class-by-class-mapping-all-37-legacy-classes)/[§11](#11-side-by-side-examples-for-common-operations) tables or editor autocomplete.
6. **Re-check parameters** for every call — several methods reordered args, changed types (`list_id` int → str), added params (`order_by`), or dropped pagination params entirely ([§11](#11-side-by-side-examples-for-common-operations), [§13](#13-endpointsmethods-removed-in-v2)).
7. **Update response handling** — the return value is now a typed `pydantic` model, not a JSON string. Delete manual `json.loads` / dict-digging. Use `*_with_http_info` when you need the status code or headers ([§7](#7-response-payloads-are-now-properly-typed)).
8. **Update error handling** — fix the `ApiException` import, optionally catch the new subclasses (`UnauthorizedException`, `BadRequestException`, …), and handle `pydantic.ValidationError` where you build requests from untrusted input ([§8](#8-error-handling-changes)).
9. **Replace `async_req=True`** usage with your own `ThreadPoolExecutor` (one `ApiClient` per worker) — the thread-pool path is gone ([§9](#9-removed-async_req-threading--plus-new-per-call-request-controls)).
10. **Check for removed endpoints and dropped products** ([§13](#13-endpointsmethods-removed-in-v2)) — the entire Fax, Letters, and Postcards products are gone — and confirm a replacement exists in the current API before shipping.
11. **Test each migrated call against ClickSend sandbox/test credentials** before deploying. Python won't catch renamed methods until runtime, so smoke-test every endpoint your integration uses.
