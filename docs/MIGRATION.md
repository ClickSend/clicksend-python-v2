# Migration Guide: clicksend-client → clicksend (Python SDK)

This guide helps you migrate an existing integration from the legacy `clicksend-client` package (v5.x) to the current `clicksend` package (v6.x).

This is not a drop-in upgrade. Package name, import paths, class names, method names, request/response objects, and error handling have all changed. Plan for a real migration effort, not a version bump — but the change list below is finite and mechanical, so most integrations can be ported endpoint-by-endpoint.

## Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Package name and imports](#package-name-and-imports)
- [Client setup and authentication](#client-setup-and-authentication)
- [Making a request](#making-a-request)
- [API classes: what moved where](#api-classes-what-moved-where)
- [Method naming](#method-naming)
- [Building request bodies](#building-request-bodies)
- [Reading responses](#reading-responses)
- [Error handling](#error-handling)
- [Asynchronous requests](#asynchronous-requests)
- [File uploads](#file-uploads)
- [Pagination](#pagination)
- [Functionality that moved or is no longer exposed](#functionality-that-moved-or-is-no-longer-exposed)
- [Migration checklist](#migration-checklist)
- [Getting help](#getting-help)

## Requirements

| | Legacy (`clicksend-client`) | Current (`clicksend`) |
|---|---|---|
| Python | 2.7, 3.4+ | 3.10+ |
| Key dependencies | `certifi`, `python-dateutil`, `six`, `urllib3` | `urllib3 >= 2.1`, `python-dateutil`, `pydantic >= 2.11`, `typing-extensions` |

If you're still on Python 2 or an early Python 3 release, you'll need to upgrade your runtime before adopting the new SDK. Request/response models are now [Pydantic](https://docs.pydantic.dev/) models, so any code that duck-types against the old plain-object models will need review.

## Installation

```sh
# Legacy
pip install clicksend-client

# Current
pip install git+https://github.com/ClickSend/clicksend-python-v2.git
```

Update your `requirements.txt` / `pyproject.toml` accordingly, and remove the old `clicksend-client` dependency — the two packages can technically coexist (different top-level module names), but keeping both around invites confusion.

## Package name and imports

The top-level module name changed from `clicksend_client` to `clicksend`.

```python
# Before
import clicksend_client
from clicksend_client.rest import ApiException

# After
import clicksend
from clicksend.rest import ApiException
```

Every import in your codebase that references `clicksend_client.*` (including model imports like `from clicksend_client.models.sms_message import SmsMessage`) needs to be updated to `clicksend.*`, and the specific model/class names should be re-checked against the tables below since many were renamed or merged.

## Client setup and authentication

Authentication is still HTTP Basic Auth using your ClickSend **username** and **API key**, but configuration is now passed via constructor arguments instead of being set as attributes after instantiation, and the API client supports use as a context manager.

```python
# Before
import clicksend_client
from clicksend_client.rest import ApiException

configuration = clicksend_client.Configuration()
configuration.username = 'YOUR_USERNAME'
configuration.password = 'YOUR_API_KEY'

api_instance = clicksend_client.SMSApi(clicksend_client.ApiClient(configuration))
```

```python
# After
import os
import clicksend
from clicksend.rest import ApiException

configuration = clicksend.Configuration(
    username=os.environ["CLICKSEND_USERNAME"],
    password=os.environ["CLICKSEND_API_KEY"],
)

with clicksend.ApiClient(configuration) as api_client:
    sms_api = clicksend.SmsApi(api_client)
    ...
```

Using `with clicksend.ApiClient(configuration) as api_client:` is the recommended pattern — it ensures the underlying connection pool is cleaned up. The old `ApiClient()` (no `with`) still works but you're responsible for closing it yourself.

The default host also changed: the legacy client pointed at `https://rest.clicksend.com/v3` by default, while the current client defaults to `https://rest.clicksend.com` (the `/v3` path prefix is now baked into each endpoint's path rather than the base host). If you previously overrode `configuration.host`, drop any trailing `/v3`.

## Making a request

The overall call shape is similar (instantiate an API class, call a method, catch `ApiException`), but three things differ: method names, the object you pass in, and the object you get back.

```python
# Before
try:
    api_response = api_instance.sms_send_post(sms_messages)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SMSApi->sms_send_post: %s\n" % e)
```

```python
# After
try:
    response = sms_api.send_sms(
        send_sms_request={
            "messages": [
                {"source": "sdk", "body": "Hello from ClickSend!", "to": "+61411111111"}
            ]
        }
    )
    print(response)
except ApiException as e:
    print(f"Exception when calling SmsApi->send_sms: {e}")
```

## API classes: what moved where

API classes were reorganized. Several legacy classes that split a feature area into "sending", "delivery receipt rules", and "inbound automation" classes have been consolidated into one class per channel. A handful of narrowly-scoped classes were merged into a broader class. Class names also switched from all-caps acronyms (`SMSApi`, `MMSApi`) to standard PascalCase (`SmsApi`, `MmsApi`). The **Fax**, **Letters**, and **Postcards** feature areas were dropped from the SDK entirely — see [Functionality that moved or is no longer exposed](#functionality-that-moved-or-is-no-longer-exposed).

| Legacy class | Current class | Notes |
|---|---|---|
| `SMSApi` | `SmsApi` | |
| `SMSDeliveryReceiptRulesApi` | `SmsApi` | Merged in |
| `InboundSMSRulesApi` | `SmsApi` | Merged in |
| `SMSCampaignApi` | `SmsCampaignsApi` | |
| `MMSApi` | `MmsApi` | |
| `MmsCampaignApi` | `MmsCampaignsApi` | |
| `FAXApi` | — | **Not present in v2** — see [Functionality that moved or is no longer exposed](#functionality-that-moved-or-is-no-longer-exposed) |
| `FAXDeliveryReceiptRulesApi` | — | **Not present in v2** |
| `InboundFAXRulesApi` | — | **Not present in v2** |
| `VoiceApi` | `VoiceApi` (rules only) + `VoiceMessagingApi` (send/history/price) | Split: `VoiceApi` now only holds delivery receipt rule methods; sending, cancelling, and history moved to `VoiceMessagingApi` |
| `VoiceDeliveryReceiptRulesApi` | `VoiceApi` | Merged in |
| `EmailMarketingApi` | `EmailApi` | |
| `TransactionalEmailApi` | `EmailApi` | Merged in |
| `MasterEmailTemplatesApi` | `EmailApi` | Merged in |
| `UserEmailTemplatesApi` | `EmailApi` | Merged in |
| `EmailDeliveryReceiptRulesApi` | `EmailApi` | Merged in |
| `EmailToSmsApi` | `EmailToSmsApi` | Same area, some methods renamed |
| `ContactApi` | `ContactsApi` | Single-contact operations |
| `ContactListApi` | `ListsApi` | List and list-contact operations |
| `SearchApi` | — | No direct SDK equivalent — see [Functionality that moved or is no longer exposed](#functionality-that-moved-or-is-no-longer-exposed) |
| `CountriesApi` | `InternationalMessagingApi` | |
| `TimezonesApi` | `InternationalMessagingApi` | Merged in |
| `GlobalSendingApi` | `InternationalMessagingApi` | Merged in |
| `NumberApi` | `NumbersApi` (buy/search) + `OwnNumbersApi` (manage/verify numbers you own) | Own-number management/OTP verification is new surface area |
| `PostLetterApi` | — | **Not present in v2** |
| `DetectAddressApi` | — | **Not present in v2** |
| `PostPostcardApi` | — | **Not present in v2** |
| `PostReturnAddressApi` | `AddressesApi` | Still present even though letters/postcards are not |
| `AccountApi` | `ManagementApi` (account info/usage) + `VerificationApi` (forgot password/username) | Account creation/self-verification endpoints removed — see below |
| `AccountRechargeApi` | `TransactionsApi` | Merged in |
| `DeliveryIssuesApi` | `MessageDeliveryApi` | |
| `ReferralAccountApi` | `ReferralsApi` | |
| `ResellerAccountApi` | `ResellerApi` | |
| `TransferCreditApi` | `ResellerApi` | Merged in |
| `SubaccountApi` | `SubaccountsApi` | |
| `UploadApi` | `UploadsApi` | Upload mechanics changed — see [File uploads](#file-uploads) |
| `StatisticsApi` | `StatisticsApi` | Unchanged name |
| — | `AlphaTagsApi` | New — alpha tag (business name sender ID) management didn't exist in the legacy SDK |

For the full current list of API classes and their methods, see the `docs/` directory in this repo (one Markdown file per class, e.g. `docs/SmsApi.md`), or browse `clicksend/api/`.

## Method naming

Legacy method names were built from the URL path plus the HTTP verb, e.g. `sms_send_post`, `sms_history_get`, `account_useage_by_subaccount_get`. Current method names read as an action on a resource, e.g. `send_sms`, `view_sms_history`. There is no mechanical rule to derive one from the other — check the relevant `docs/<ClassName>.md` file or the table below for the endpoints you use.

Common endpoints:

| Legacy class.method | Current class.method |
|---|---|
| `AccountApi.account_get` | `ManagementApi.view_account_details` |
| `AccountApi.account_useage_by_subaccount_get` | `ManagementApi.view_account_usage` |
| `AccountApi.forgot_password_put` | `VerificationApi.forgot_password` |
| `AccountApi.forgot_username_put` | `VerificationApi.forgot_username` |
| `SMSApi.sms_send_post` | `SmsApi.send_sms` |
| `SMSApi.sms_history_get` | `SmsApi.view_sms_history` |
| `SMSApi.sms_price_post` | `SmsApi.calculate_sms_price` |
| `SMSApi.sms_receipts_get` | `SmsApi.view_sms_receipts` |
| `SMSApi.sms_cancel_all_put` | `SmsApi.cancel_all_sms` |
| `MMSApi.mms_send_post` | `MmsApi.send_mms` |
| `MMSApi.mms_history_get` | `MmsApi.view_mms_history` |
| `MMSApi.mms_price_post` | `MmsApi.calculate_mms_price` |
| `VoiceApi.voice_send_post` | `VoiceMessagingApi.send_voice_message` |
| `EmailMarketingApi.email_campaign_post` | `EmailApi.send_email_campaign` |
| `TransactionalEmailApi.email_send_post` | `EmailApi.send_email` |
| `SubaccountApi.subaccounts_post` | `SubaccountsApi.create_subaccount` |
| `TransferCreditApi.reseller_transfer_credit_put` | `ResellerApi.reseller_transfer_credit` |
| `ContactApi.lists_contacts_by_list_id_post` | `ListsApi.create_new_contact` |
| `ContactListApi.lists_post` | `ListsApi.create_list` |
| `ContactListApi.lists_get` | `ListsApi.view_lists` |
| `UploadApi.uploads_post` | `UploadsApi.upload_a_media_file` |

## Building request bodies

Legacy models were hand-rolled classes: you instantiated an empty model and assigned attributes, or passed positional arguments, and wrapped multi-item payloads in a `*Collection` class.

```python
# Before
sms_message = clicksend_client.SmsMessage()
sms_message.source = 'sdk'
sms_message.body = 'Hello from ClickSend!'
sms_message.to = '+61411111111'

sms_messages = clicksend_client.SmsMessageCollection()
sms_messages.messages = [sms_message]

api_response = api_instance.sms_send_post(sms_messages)
```

Current models are Pydantic models. You can construct them explicitly, or — as shown in the SDK's own examples — just pass a plain `dict` with the right shape and let the SDK validate/coerce it:

```python
# After — explicit model
from clicksend.models.send_sms_request import SendSmsRequest
from clicksend.models.send_sms_request_messages_inner import SendSmsRequestMessagesInner

request = SendSmsRequest(
    messages=[
        SendSmsRequestMessagesInner(source="sdk", body="Hello from ClickSend!", to="+61411111111"),
    ]
)
response = sms_api.send_sms(send_sms_request=request)

# After — plain dict (also valid)
response = sms_api.send_sms(
    send_sms_request={
        "messages": [
            {"source": "sdk", "body": "Hello from ClickSend!", "to": "+61411111111"},
        ]
    }
)
```

There's no more `*Collection` wrapper class — the request model itself has a `messages` (or equivalent) list field.

A few endpoints, such as `send_sms` and `upload_a_media_file`, also accept an optional `content_type` parameter. This overrides the `Content-Type` header for that single call and is unrelated to the request body — you generally don't need to set it.

## Reading responses

This is one of the most impactful changes for existing code: **legacy `*_post`/`*_get` methods returned a raw JSON string**, which you had to `json.loads()` yourself to get at the data. **Current methods return a typed, already-parsed model object** with real attributes.

```python
# Before
import json

raw = api_instance.sms_send_post(sms_messages)   # returns str
parsed = json.loads(raw)
message_id = parsed['data']['messages'][0]['message_id']
```

```python
# After
response = sms_api.send_sms(send_sms_request=request)  # returns SendSms
message_id = response.data.messages[0].message_id
```

Response models also give you `.to_dict()` and `.to_json()` if you need to serialize them (e.g. for logging), and `.model_dump()` since they're Pydantic models under the hood. Audit any code that does manual `json.loads(...)` or dict-key access (`response['data']['...']`) on SDK return values — that code will break, since it now receives an object rather than a string.

## Error handling

Both versions raise on non-2xx responses via `ApiException`, importable from `clicksend.rest` (previously `clicksend_client.rest`), and both expose `.status`, `.reason`, `.body`, and `.headers`.

The current SDK adds:
- A `.data` attribute holding the parsed error payload (when available), alongside the raw `.body` string.
- Status-specific subclasses raised automatically based on the HTTP status code: `BadRequestException` (400), `UnauthorizedException` (401), `ForbiddenException` (403), `NotFoundException` (404), `ConflictException` (409), `UnprocessableEntityException` (422), `ServiceException` (5xx). All still inherit from `ApiException`, so existing `except ApiException:` blocks keep working unchanged — but you can now catch specific cases if useful.

```python
# Works in both versions
try:
    sms_api.send_sms(send_sms_request=request)
except ApiException as e:
    print(f"{e.status}: {e.reason}")
```

```python
# New in current SDK — narrower catch if you want it
from clicksend.exceptions import UnauthorizedException

try:
    sms_api.send_sms(send_sms_request=request)
except UnauthorizedException as e:
    print(f"Bad credentials: {e.data}")
```

## Asynchronous requests

The legacy client accepted `async_req=True` on every method, which dispatched the call on an internal thread pool and returned a handle you'd call `.get()` on:

```python
# Before — legacy-only, no equivalent in the current SDK
thread = api_instance.sms_send_post(sms_messages, async_req=True)
result = thread.get()
```

**This parameter does not exist in the current SDK.** All calls are synchronous. If you relied on `async_req` for concurrency, replace it with your own threading, e.g. `concurrent.futures.ThreadPoolExecutor`, wrapping calls to the (synchronous) SDK methods.

## File uploads

The legacy `UploadApi.uploads_post` accepted an `UploadFile` model representing a `multipart/form-data` file upload, plus a separate `convert` string argument.

The current `UploadsApi.upload_a_media_file` takes a JSON `body` containing the base64-encoded file contents and the target format:

```python
# Before
upload_file = clicksend_client.UploadFile()
# ... populate with your file's bytes ...
api_response = api_instance.uploads_post(upload_file, 'mms')
```

```python
# After
import base64

with open('image.jpg', 'rb') as f:
    encoded = base64.b64encode(f.read()).decode('utf-8')

api_instance.upload_a_media_file(
    body={"content": encoded, "convert": "mms"}
)
```

Any code that streams or reads files for upload will need to add a base64-encoding step.

## Pagination

List/history endpoints in both SDKs support a `page` parameter. In the legacy SDK it was an untyped keyword argument passed through `**kwargs`. In the current SDK it's an explicit, typed parameter on the method signature (default `1`), so it now shows up in autocomplete and is validated client-side:

```python
# Before
api_instance.sms_history_get(page=2)

# After
sms_api.view_sms_history(page=2)
```

## Functionality that moved or is no longer exposed

A few legacy endpoints don't have a direct equivalent in the current SDK's surface:

- **Fax** — the entire feature area is gone. `FAXApi` (send/history/price/receipts), `FAXDeliveryReceiptRulesApi`, and `InboundFAXRulesApi` have no v2 class, and there are no fax models. There is no `send_fax` equivalent.
- **Letters** — the entire feature area is gone. `PostLetterApi` (send/history/export/price) has no v2 class, and there are no letter models.
- **Postcards** — the entire feature area is gone. `PostPostcardApi` (send/history/export/price) has no v2 class, and there are no postcard models.
- **Address detection** (`DetectAddressApi.detect_address_post`) — no equivalent in the current SDK. (`PostReturnAddressApi` did survive, as `AddressesApi`.)
- **Self-service account creation and verification** (`AccountApi.account_post`, `account_verify_send_put`, `account_verify_verify_by_activation_token_put`) — not present in the current SDK. Account creation/activation is handled outside the API.
- **Contact/list search** (`SearchApi.search_contacts_lists_get`) — no equivalent method exists in the current SDK.

If your integration depends on either of these, check with ClickSend support before migrating rather than assuming a silent replacement exists.

Conversely, the current SDK adds functionality that didn't exist in the legacy client, notably **`OwnNumbersApi`** (manage and OTP-verify numbers you own, outside of ClickSend-purchased dedicated numbers).

## Migration checklist

1. Upgrade to Python 3.10+ if you haven't already.
2. Replace the `clicksend-client` dependency with `clicksend` and update every `import clicksend_client` / `from clicksend_client...` to `clicksend`.
3. Update configuration/client setup to pass `username`/`password` into `clicksend.Configuration(...)` directly, and adopt the `with clicksend.ApiClient(configuration) as api_client:` pattern.
4. Re-point each API class instantiation at its new class name (see the [class mapping table](#api-classes-what-moved-where)).
5. Re-point each method call at its new method name (see [Method naming](#method-naming) and the per-class `docs/*.md` files).
6. Replace hand-built model objects with the new Pydantic models or equivalent dicts.
7. Remove any `json.loads(...)` calls on SDK responses — access fields directly on the returned model instead.
8. Remove any `async_req=True` usage and replace with your own concurrency if needed.
9. Update any file-upload code to base64-encode content instead of passing a file/multipart object.
10. Re-test error handling paths — confirm `except ApiException` still catches what you expect, and optionally adopt the new status-specific subclasses.
11. Run your integration against a test ClickSend account end-to-end before deploying.

## Getting help

- Full current API reference: https://developers.clicksend.com/docs/rest/v3/
- Per-class/method usage examples: the `docs/` directory in this repository
- Support: https://clicksend.com/contact or the [Help Centre](https://help.clicksend.com/)
