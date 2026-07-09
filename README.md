# ClickSend Python SDK

Official Python client for the [ClickSend API](https://developers.clicksend.com/) — send and manage SMS, MMS, email, voice, fax, letters, postcards, and more.

## Requirements

Python 3.10+

## Installation

```sh
pip install git+https://github.com/ClickSend/clicksend-python-v2.git
```

## Getting Started

```python
import clicksend
from clicksend.rest import ApiException

configuration = clicksend.Configuration(
    username=os.environ["CLICKSEND_USERNAME"],
    password=os.environ["CLICKSEND_API_KEY"],
)

with clicksend.ApiClient(configuration) as api_client:
    sms_api = clicksend.SmsApi(api_client)

    try:
        response = sms_api.sms_send_post(
            sms_message_collection={
                "messages": [
                    {"source": "sdk", "body": "Hello from ClickSend!", "to": "+61411111111"}
                ]
            }
        )
        print(response)
    except ApiException as e:
        print(f"Exception when calling SmsApi->sms_send_post: {e}")
```

## Authentication

The API uses HTTP Basic authentication — your ClickSend **username** and **API key** (available from the [ClickSend Dashboard](https://dashboard.clicksend.com/#/account/subaccount)).

## Documentation

Full API reference: https://developers.clicksend.com/docs/rest/v3/

## Support

Need help? Contact [ClickSend Support](https://clicksend.com/contact) or visit the [Help Centre](https://help.clicksend.com/).
