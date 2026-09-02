# ClickSend Python SDK v6.0.0

The first release of the **next-generation ClickSend Python SDK**, published from the new [`clicksend-python-v2`](https://github.com/ClickSend/clicksend-python-v2) repository.

This SDK is built fresh against ClickSend's current REST API, replacing the previous `clicksend-client` package. Although it lives in a new repo, it continues the version line of the legacy `clicksend-client` package (previously `5.x`) — hence **6.0.0**, a major bump signalling breaking changes.

> ⚠️ **This is not a drop-in replacement.** Package name, import paths, method names, request/response shapes, class groupings, and error handling have all changed. Read the [Migration Guide](https://github.com/ClickSend/clicksend-python-v2/blob/main/docs/MIGRATION.md) before upgrading.

## Installation

```sh
pip install clicksend==6.0.0
```

Also installable from source:

```sh
pip install git+https://github.com/ClickSend/clicksend-python-v2.git
```

## What's new

- **Resource-oriented API classes** — 26 classes, one per resource/tag (`SmsApi`, `MmsApi`, `EmailApi`, `VoiceMessagingApi`, `ContactsApi`, `ListsApi`, …), down from 37 loosely-grouped legacy classes. Several legacy classes were merged (five email classes → one `EmailApi`; SMS/Voice/Email delivery-receipt-rule and inbound-rule classes folded into their channel class); Voice was split; and the Fax, Letters, and Postcards classes were dropped entirely.
- **Readable method names** — methods are now named after what they do (`send_sms`, `view_sms_history`, `export_sms_history`) instead of the old `resource_path_http_verb` pattern (`sms_send_post`, `sms_history_get`).
- **Pydantic v2 request models** — every operation takes a dedicated `*Request` model (`SendSmsRequest`, `CreateSubaccountRequest`, …) instead of hand-rolled reusable domain models. A plain `dict` with the right shape is also accepted and is validated/coerced by the model.
- **Typed response models** — response bodies are deserialized into specific Pydantic models (`SendSms`, `ViewSmsHistory`, …) with real attributes, plus `.to_dict()`, `.to_json()`, and `.model_dump()`. No more `json.loads()` on a raw string.
- **Real exception classes** — non-2xx responses raise `ApiException` exposing `.status`, `.reason`, `.body`, `.headers`, and a new `.data` holding the parsed error payload, instead of returning a raw JSON string.
- **Status-specific exception subclasses** — `BadRequestException` (400), `UnauthorizedException` (401), `ForbiddenException` (403), `NotFoundException` (404), `ConflictException` (409), `UnprocessableEntityException` (422), and `ServiceException` (5xx), all raised automatically and all subclasses of `ApiException`, so existing `except ApiException:` blocks keep working.
- **Context-manager client** — `with clicksend.ApiClient(configuration) as api_client:` cleans up the underlying connection pool for you.
- **Per-call response variants** — every method has `*_with_http_info` (returns status code + headers) and `*_without_preload_content` (returns the raw undecoded `urllib3` response) siblings.
- **Constructor-based configuration** — `clicksend.Configuration(username=..., password=...)`, plus `api_key` / `access_token` slots and per-call `_headers`, `_request_timeout`, and `_request_auth` overrides.
- **Ships `py.typed`** — inline type hints usable by mypy and IDEs.

## New resources and methods (no legacy equivalent)

- `AlphaTagsApi` — list / get / request / delete alpha tags
- `DefaultSendersApi` — manage default sender IDs and list compliant sender types
- `OwnNumbersApi` — Bring Your Own Number: list, detail, update, delete, request/verify OTP
- `UrlShorteningApi` — short-URL statistics and tracking
- `NumbersApi.register_numbers` — number registration
- `SubaccountsApi.generate_new_api_key` — rotate a subaccount API key
- `SmsApi.view_a_specific_inbound_sms_message`, `SmsApi.view_a_specific_sms_template` — fetch a single record by ID

## Breaking changes

- Package name is `clicksend` (PyPI) and the import root is `clicksend`; the legacy `clicksend-client` package / `clicksend_client` module is no longer published from this line. Update every `import clicksend_client` / `from clicksend_client...` (including model imports) and `from clicksend_client.rest import ApiException` → `from clicksend.rest import ApiException`.
- Every API class and method has been renamed — no mechanical find-and-replace works. Acronym class names (`SMSApi`, `MMSApi`) → PascalCase (`SmsApi`, `MmsApi`); method names (`sms_send_post`) → action-first (`send_sms`). See the [class-by-class mapping](https://github.com/ClickSend/clicksend-python-v2/blob/main/docs/MIGRATION.md#api-classes-what-moved-where).
- ⚠️ **Voice naming trap:** legacy `VoiceApi` (sending) → new **`VoiceMessagingApi`**; legacy `VoiceDeliveryReceiptRulesApi` → new **`VoiceApi`**. The new `VoiceApi` does *not* send voice calls.
- Default host changed from `https://rest.clicksend.com/v3` to `https://rest.clicksend.com`; the `/v3` prefix is now part of each method path. Drop any trailing `/v3` from a custom `host`.
- Authentication is configured via constructor kwargs — `clicksend.Configuration(username=..., password=...)` — instead of assigning `configuration.username` / `configuration.password` after construction.
- Responses are typed models, not `str` — any code doing `json.loads(response)` or `response['data'][...]` on a return value breaks; use attribute access (`response.data.messages[0].message_id`).
- Request bodies are Pydantic models or dicts — the hand-built model objects and `*Collection` wrapper classes (`SmsMessageCollection`, …) are gone; the request model carries the `messages` (or equivalent) list directly.
- `async_req=True` has been removed — all calls are synchronous. Use your own `concurrent.futures.ThreadPoolExecutor` for concurrency.
- File uploads changed — `UploadApi.uploads_post(UploadFile, 'mms')` (`multipart/form-data`) → `UploadsApi.upload_a_media_file(body={"content": <base64>, "convert": "mms"})` (JSON with base64-encoded contents).
- Every method takes a leading `content_type: Optional[str] = None` argument for the `Content-Type` header.
- Pagination parameters (`page`, `limit`) were dropped from several method signatures, including `ListsApi.view_lists`, `ListsApi.view_list_contacts`, and `SubaccountsApi.view_subaccounts`. They remain on history endpoints such as `SmsApi.view_sms_history` (now explicit, typed keyword arguments rather than untyped `**kwargs`).
- **Fax, Letters, and Postcards are not part of the v2 SDK** — the `FAXApi` / `FAXDeliveryReceiptRulesApi` / `InboundFAXRulesApi`, `PostLetterApi`, and `PostPostcardApi` classes (and all their models) have no v2 equivalent. `DetectAddressApi` and `SearchApi` were also dropped.
- Some other legacy endpoints have no v2 equivalent (self-service account creation/verification, and various receipt-read / test-receipt operations) — see [Functionality that moved or is no longer exposed](https://github.com/ClickSend/clicksend-python-v2/blob/main/docs/MIGRATION.md#functionality-that-moved-or-is-no-longer-exposed).
- `six` and `certifi` are no longer direct dependencies; `pydantic >= 2.11` and `typing-extensions` are now required.

## Requirements

- Python 3.10+ (Python 2.7 and 3.4–3.9 are no longer supported)
- Depends on `urllib3 >= 2.1`, `python-dateutil`, `pydantic >= 2.11`, `typing-extensions`

## Migration

Full guide: [docs/MIGRATION.md](https://github.com/ClickSend/clicksend-python-v2/blob/main/docs/MIGRATION.md) — covers imports, auth, base paths, the naming convention change, request/response model changes, error handling, the complete legacy→v2 class map, side-by-side examples, and a step-by-step checklist.
