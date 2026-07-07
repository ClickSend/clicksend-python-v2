# clicksend.VoiceMessagingOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_voice_price**](VoiceMessagingOtherApi.md#calculate_voice_price) | **POST** /v3/voice/price | Calculate Voice Price
[**cancel_all_voice_messages**](VoiceMessagingOtherApi.md#cancel_all_voice_messages) | **PUT** /v3/voice/cancel-all | Cancel All Voice Messages
[**cancel_voice_message**](VoiceMessagingOtherApi.md#cancel_voice_message) | **PUT** /v3/voice/{message_id}/cancel | Cancel Voice Message
[**export_voice_history**](VoiceMessagingOtherApi.md#export_voice_history) | **GET** /v3/voice/history/export | Export Voice History
[**get_voice_history**](VoiceMessagingOtherApi.md#get_voice_history) | **GET** /v3/voice/history | Get Voice History
[**send_voice_message**](VoiceMessagingOtherApi.md#send_voice_message) | **POST** /v3/voice/send | Send Voice Message
[**view_voice_languages**](VoiceMessagingOtherApi.md#view_voice_languages) | **GET** /v3/voice/lang | View Voice Languages
[**view_voice_receipts**](VoiceMessagingOtherApi.md#view_voice_receipts) | **GET** /v3/voice/receipts | View Voice Receipts


# **calculate_voice_price**
> CalculateVoicePrice calculate_voice_price(content_type=content_type, calculate_voice_price_request=calculate_voice_price_request)

Calculate Voice Price

_Calculate voice price_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| body | string | true | none | Biscuit uv3nlCOjRk croissant chocolate lollipop chocolate muffin. |
| voice | string | true | none | Either 'female' or 'male'. |
| custom_string | string | true | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | true | none | The country of the recipient. |
| source | string | false | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| lang | string | false | none | au (string, required) - See section on available languages. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| require_input | integer(int1) | false | none | Recieve a keypress from the recipient. Flag value must be 1 for yes or 0 for no. |
| machine_detection | integer(int1) | false | none | Detect answering machine or voicemail and leave a message. Flag value must be 1 for yes or 0 for no. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_voice_price import CalculateVoicePrice
from clicksend.models.calculate_voice_price_request import CalculateVoicePriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_voice_price_request = clicksend.CalculateVoicePriceRequest() # CalculateVoicePriceRequest |  (optional)

    try:
        # Calculate Voice Price
        api_response = api_instance.calculate_voice_price(content_type=content_type, calculate_voice_price_request=calculate_voice_price_request)
        print("The response of VoiceMessagingOtherApi->calculate_voice_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->calculate_voice_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_voice_price_request** | [**CalculateVoicePriceRequest**](CalculateVoicePriceRequest.md)|  | [optional] 

### Return type

[**CalculateVoicePrice**](CalculateVoicePrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_all_voice_messages**
> CancelAllVoiceMessages cancel_all_voice_messages(content_type=content_type, body=body)

Cancel All Voice Messages

_Update all voice messages as cancelled_

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_all_voice_messages import CancelAllVoiceMessages
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Cancel All Voice Messages
        api_response = api_instance.cancel_all_voice_messages(content_type=content_type, body=body)
        print("The response of VoiceMessagingOtherApi->cancel_all_voice_messages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->cancel_all_voice_messages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CancelAllVoiceMessages**](CancelAllVoiceMessages.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_voice_message**
> CancelVoiceMessage cancel_voice_message(message_id, content_type=content_type, body=body)

Cancel Voice Message

_Update voice message status as cancelled_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | path | string | true | Your voice message id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_voice_message import CancelVoiceMessage
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    message_id = 'message_id_example' # str | 
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Cancel Voice Message
        api_response = api_instance.cancel_voice_message(message_id, content_type=content_type, body=body)
        print("The response of VoiceMessagingOtherApi->cancel_voice_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->cancel_voice_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CancelVoiceMessage**](CancelVoiceMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_voice_history**
> ExportVoiceHistory export_voice_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)

Export Voice History

_Export voice history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to export to |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_voice_history import ExportVoiceHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    filename = 'Voice_history.csv' # str |  (optional)
    q = 'q_example' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 50000 # int |  (optional)

    try:
        # Export Voice History
        api_response = api_instance.export_voice_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)
        print("The response of VoiceMessagingOtherApi->export_voice_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->export_voice_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **filename** | **str**|  | [optional] 
 **q** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 
 **date_from** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 

### Return type

[**ExportVoiceHistory**](ExportVoiceHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_voice_history**
> GetVoiceHistory get_voice_history(content_type=content_type, date_to=date_to, limit=limit, operator=operator, order_by=order_by, page=page)

Get Voice History

_Get all voice history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_voice_history import GetVoiceHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 20 # int |  (optional)
    operator = 'AND' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    page = 1 # int |  (optional)

    try:
        # Get Voice History
        api_response = api_instance.get_voice_history(content_type=content_type, date_to=date_to, limit=limit, operator=operator, order_by=order_by, page=page)
        print("The response of VoiceMessagingOtherApi->get_voice_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->get_voice_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 
 **operator** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 
 **page** | **int**|  | [optional] 

### Return type

[**GetVoiceHistory**](GetVoiceHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_voice_message**
> SendVoiceMessage send_voice_message(content_type=content_type, send_voice_message_request=send_voice_message_request)

Send Voice Message

_Send voice message(s)_

Send TTS (Text-to-speech) voice calls

### How many messages can I send?

You can post **up to 1000 messages** with each API call. You can send to a mix of contacts and contact lists, as long as the total number of recipients is up to 1000. The response contains a status and details for each recipient.

### How many characters can I send in a message?

If a message is longer than 4 message parts, it will be truncated (see below). If a message contains any characters that aren't in the GSM 03.38 character set, the message type will be treated as unicode. (`https://en.wikipedia.org/wiki/GSM_03.38`)

### _Standard English Characters:_

| Number of Characters | Message Credits |
| --- | --- |
| 1 - 300 | 1 |
| 301 - 600 | 2 |
| 601 - 900 | 3 |
| 901 - 1200 | 4 |

### _Non-GSM (Unicode) characters:_

| Number of Characters | Message Credits |
| --- | --- |
| 1 - 150 | 1 |
| 151 - 300 | 2 |
| 301 - 450 | 3 |
| 451 - 600 | 4 |

### _Allowed Languages_

| Language, Locale | lang | voice |
| --- | --- | --- |
| `English`, US | en-us | female (default) / male |
| `English`, Australia | en-au | female (default) / male |
| `English`, UK | en-gb | female (default) / male |
| `English`, India | en-in | female |
| `English`, Wales | en-gb-wls | female (default) / male |
| `Celtic`, Wales | cy-gb-wls | female (default) / male |
| `German`, Germany | de-de | female (default) / male |
| `Spanish`, Spain | es-es | female (default) / male |
| `Spanish`, US | es-us | female (default) / male |
| `French`, Canada | fr-ca | female |
| `French`, France | fr-fr | female (default) / male |
| `Icelandic`, Iceland | is-is | female (default) / male |
| `Italian`, Italy | it-it | female (default) / male |
| `Danish`, Denmark | da-dk | female (default) / male |
| `Dutch`, Netherlands | nl-nl | female (default) / male |
| `Norwegian`, Norway | nb-no | female |
| `Polish`, Poland | pl-pl | female (default) / male |
| `Portuguese`, Portugal | pt-pt | male |
| `Portuguese`, Brazil | pt-br | female (default) / male |
| `Romanian`, Romania | ro-ro | female |
| `Russian`, Russia | ru-ru | female (default) / male |
| `Swedish`, Sweden | sv-se | female |
| `Turkish`, Turkey | tr-tr | female |

_Tips_

To introduce a small delay between words or digits you can use a comma (,).

For example: `Please enter your activation code 9, 0, 9, 0, in the next 20 minutes.`

We support some SSML tags allowing custom breaks or pauses to be entered, and the readout rate to be altered.

[More info...](https://help.clicksend.com/en/articles/42982-customising-text-to-voice-output)

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| body | string | true | none | Biscuit uv3nlCOjRk croissant chocolate lollipop chocolate muffin. |
| voice | string | true | none | Either 'female' or 'male'. |
| custom_string | string | true | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | true | none | The country of the recipient. |
| source | string | false | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| lang | string | false | none | au (string, required) - See section on available languages. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| require_input | integer(int1) | false | none | Recieve a keypress from the recipient. Flag value must be 1 for yes or 0 for no. |
| machine_detection | integer(int1) | false | none | Detect answering machine or voicemail and leave a message. Flag value must be 1 for yes or 0 for no. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_voice_message import SendVoiceMessage
from clicksend.models.send_voice_message_request import SendVoiceMessageRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_voice_message_request = clicksend.SendVoiceMessageRequest() # SendVoiceMessageRequest |  (optional)

    try:
        # Send Voice Message
        api_response = api_instance.send_voice_message(content_type=content_type, send_voice_message_request=send_voice_message_request)
        print("The response of VoiceMessagingOtherApi->send_voice_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->send_voice_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_voice_message_request** | [**SendVoiceMessageRequest**](SendVoiceMessageRequest.md)|  | [optional] 

### Return type

[**SendVoiceMessage**](SendVoiceMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_voice_languages**
> ViewVoiceLanguages view_voice_languages(content_type=content_type)

View Voice Languages

_Get all voice languages_


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_languages import ViewVoiceLanguages
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Languages
        api_response = api_instance.view_voice_languages(content_type=content_type)
        print("The response of VoiceMessagingOtherApi->view_voice_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->view_voice_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceLanguages**](ViewVoiceLanguages.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_voice_receipts**
> ViewVoiceReceipts view_voice_receipts(content_type=content_type)

View Voice Receipts

_Get all voice receipts_

**Push Delivery Receipts**

If you prefer, we can push message replies to your server as they arrive with us.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Voice then Delivery Report Rules.
5. Click the 'Add New Rule' button.
6. Select the 'URL' action.
7. Enter the URL and click 'Save'.
    

The following variables will be posted to the URL specified:

| Variable | Description |
| --- | --- |
| `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980 |
| `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981 |
| `message_id` | Message ID, returned when originally sending the message. |
| `status` | Delivered or Undelivered |
| `status_code` | Status code. Refer to 'Voice Delivery Status Codes' in docs. |
| `status_text` | Status text. |
| `error_code` | Error code. |
| `error_text` | Error text. |
| `custom_string` | A custom string used when sending the original message. |
| `user_id` | The user ID of the user who sent the message. |
| `subaccount_id` | The subaccount ID of the user who sent the message. |
| `message_type` | 'voice' (constant). |
| `digits` | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn't provide any input. |

**Pull Delivery Receipts**

Receive delivery reports by polling. You can poll our server and retrieve delivery reports at a time that suits you.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Voice then Delivery Report Rules.
5. Click the 'Add New Rule' button.
6. Select the 'Poll' action.
7. Then click 'Save'.
    

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_receipts import ViewVoiceReceipts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.VoiceMessagingOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Receipts
        api_response = api_instance.view_voice_receipts(content_type=content_type)
        print("The response of VoiceMessagingOtherApi->view_voice_receipts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceMessagingOtherApi->view_voice_receipts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceReceipts**](ViewVoiceReceipts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

