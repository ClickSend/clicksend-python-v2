# ClickSend Python SDK

[![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![API: v3](https://img.shields.io/badge/ClickSend%20API-v3-brightgreen.svg)](https://developers.clicksend.com/docs/rest/v3/)

Official Python client for the [ClickSend API](https://developers.clicksend.com/) — send SMS, MMS, voice and email messages, run SMS and MMS campaigns, manage numbers, contacts and subaccounts, and pull delivery receipts and reporting through a single authenticated HTTPS client.

This library is generated from ClickSend's official OpenAPI v3 specification and is maintained by ClickSend. It covers every endpoint of the [ClickSend REST API](https://developers.clicksend.com/docs/rest/v3/).

- 📚 **API reference:** https://developers.clicksend.com/docs/rest/v3/
- 🔑 **Dashboard & API credentials:** https://dashboard.clicksend.com
- 🗂 **Source & issues:** https://github.com/ClickSend/clicksend-python-v2
- 💬 **Support:** https://help.clicksend.com

## Features

- **Messaging** — SMS, MMS, voice / text-to-speech, transactional email, email-to-SMS
- **Campaigns** — SMS and MMS campaigns
- **Numbers & sender IDs** — dedicated numbers, own numbers, alpha tags, default senders
- **Contacts** — contact lists, contacts and the address book
- **Account & billing** — account details, transactions, subaccounts, referrals, reseller accounts
- **Delivery & reporting** — delivery receipts, inbound messages, statistics
- **Extras** — URL shortening, file uploads, number verification, international messaging
- **Typed models** with `pydantic` validation for every request and response
- **HTTP Basic auth** with your ClickSend username and API key
- **Identifiable traffic** — requests are sent with a `ClickSend-SDK/<version>/python` `User-Agent` by default
- MIT licensed

## Requirements

- Python 3.10 or newer

## Installation

```sh
pip install clicksend-client
```

## Authentication

Every API class authenticates with HTTP Basic auth using your ClickSend **username** and **API key**, both available from the [ClickSend Dashboard](https://dashboard.clicksend.com/#/account/subaccount). Supply them through environment variables rather than hard-coding them:

```sh
export CLICKSEND_USERNAME="your-username"
export CLICKSEND_API_KEY="your-api-key"
```

## Quickstart

```python
import os
import clicksend
from clicksend.rest import ApiException

configuration = clicksend.Configuration(
    username=os.environ["CLICKSEND_USERNAME"],
    password=os.environ["CLICKSEND_API_KEY"],
)

with clicksend.ApiClient(configuration) as api_client:
    sms_api = clicksend.SmsApi(api_client)

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

## More Examples

### View account details

```python
with clicksend.ApiClient(configuration) as api_client:
    management_api = clicksend.ManagementApi(api_client)

    try:
        account = management_api.view_account_details()
        print(account)
    except ApiException as e:
        print(f"Exception when calling ManagementApi->view_account_details: {e}")
```

### Send an MMS

```python
with clicksend.ApiClient(configuration) as api_client:
    mms_api = clicksend.MmsApi(api_client)

    try:
        response = mms_api.send_mms(
            send_mms_request={
                "media_file": "https://clicksend.com/logo.png",
                "messages": [
                    {
                        "to": "+61411111111",
                        "from": "sdk",
                        "subject": "Hello",
                        "body": "Hello from ClickSend!",
                        "source": "sdk",
                    }
                ],
            }
        )
        print(response)
    except ApiException as e:
        print(f"Exception when calling MmsApi->send_mms: {e}")
```

## Configuration

```python
configuration = clicksend.Configuration(
    username=os.environ["CLICKSEND_USERNAME"],
    password=os.environ["CLICKSEND_API_KEY"],
    # Override the API base URL (default: https://rest.clicksend.com).
    host="https://rest.clicksend.com",
)
```

## Error Handling

Non-2xx responses raise `clicksend.rest.ApiException`:

```python
from clicksend.rest import ApiException

try:
    response = sms_api.send_sms(send_sms_request={"messages": [...]})
except ApiException as e:
    print(e.status)   # HTTP status code
    print(e.body)     # raw error payload from the API
    print(e.headers)  # response headers
```

## Documentation

- Full REST API reference: https://developers.clicksend.com/docs/rest/v3/
- Per-endpoint SDK docs: the [`docs/`](docs) directory in this repository
- Source code: https://github.com/ClickSend/clicksend-python-v2

## Versioning

This package follows [semantic versioning](https://semver.org/). Breaking changes are released as major versions.

## Support

- Help Centre: https://help.clicksend.com
- Contact support: https://clicksend.com/contact
- SDK bugs and feature requests: https://github.com/ClickSend/clicksend-python-v2/issues

## License

Released under the [MIT License](https://opensource.org/licenses/MIT).

---

**Keywords:** clicksend, sms, sms api, send sms, bulk sms, text message, texting, mms, mms api, voice, voice call, text to speech, tts, ivr, email to sms, sms campaign, mms campaign, url shortening, number verification, messaging, notifications, otp, 2fa, two factor authentication, transactional sms, marketing sms, appointment reminders, alerts, python, python3, rest api, clicksend sdk
