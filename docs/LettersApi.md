# clicksend.LettersApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_letter_price**](LettersApi.md#calculate_letter_price) | **POST** /v3/post/letters/price | Calculate Letter Price
[**cancel_scheduled_letter**](LettersApi.md#cancel_scheduled_letter) | **PUT** /v3/post/letters/{message_id}/cancel | Cancel Scheduled Letter
[**detect_address**](LettersApi.md#detect_address) | **POST** /v3/post/letters/detect-address | Detect Address
[**export_letter_history**](LettersApi.md#export_letter_history) | **GET** /v3/post/letters/history/export | Export Letter History
[**send_letter**](LettersApi.md#send_letter) | **POST** /v3/post/letters/send | Send Letter
[**view_letter_history**](LettersApi.md#view_letter_history) | **GET** /v3/post/letters/history | View Letter History


# **calculate_letter_price**
> CalculateLetterPrice calculate_letter_price(content_type=content_type, calculate_letter_price_request=calculate_letter_price_request)

Calculate Letter Price

_Calculate letter price_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |
| template_used | integer(int1) | false | none | Whether using our letter template. Flag value must be 1 for yes or 0 for no. |
| duplex | integer(int1) | false | none | Whether letter is duplex. Flag value must be 1 for yes or 0 for no. |
| colour | integer(int1) | false | none | Whether letter is in colour. Flag value must be 1 for yes or 0 for no. |
| priority_post | integer(int1) | false | none | Whether letter is priority. Flag value must be 1 for yes or 0 for no. |
| source | string | false | none | Source being sent from |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_letter_price import CalculateLetterPrice
from clicksend.models.calculate_letter_price_request import CalculateLetterPriceRequest
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
    api_instance = clicksend.LettersApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_letter_price_request = clicksend.CalculateLetterPriceRequest() # CalculateLetterPriceRequest |  (optional)

    try:
        # Calculate Letter Price
        api_response = api_instance.calculate_letter_price(content_type=content_type, calculate_letter_price_request=calculate_letter_price_request)
        print("The response of LettersApi->calculate_letter_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LettersApi->calculate_letter_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_letter_price_request** | [**CalculateLetterPriceRequest**](CalculateLetterPriceRequest.md)|  | [optional] 

### Return type

[**CalculateLetterPrice**](CalculateLetterPrice.md)

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

# **cancel_scheduled_letter**
> CancelScheduledLetter cancel_scheduled_letter(message_id)

Cancel Scheduled Letter

_Cancel scheduled letter_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | query | string | true | Message ID of the scheduled letter that is to be cancelled. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example


```python
import clicksend
from clicksend.models.cancel_scheduled_letter import CancelScheduledLetter
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)


# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.LettersApi(api_client)
    message_id = 'message_id_example' # str | 

    try:
        # Cancel Scheduled Letter
        api_response = api_instance.cancel_scheduled_letter(message_id)
        print("The response of LettersApi->cancel_scheduled_letter:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LettersApi->cancel_scheduled_letter: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 

### Return type

[**CancelScheduledLetter**](CancelScheduledLetter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detect_address**
> DetectAddress detect_address(content_type=content_type, body=body)

Detect Address

_Detects address in uploaded file._

The `detect-address` endpoint accepts either a letter in PDF format or an address string and attempts to convert it to a standard address format. Note that the PDF should be in standard address format, having the recipient's name and address listed at the top.

The endpoint accepts two types of data: 1. A PDF file in `base64` encoding. In this case, submit the `base64`\-encoded PDF file contents in the `content` field of the request body. 2. An address string. In this case, submit the address in a string using the `address` field of the request body.

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| convert | query | string | true | none |
| content | body | string | true | Base64-encoded file contents |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.detect_address import DetectAddress
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
    api_instance = clicksend.LettersApi(api_client)
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Detect Address
        api_response = api_instance.detect_address(content_type=content_type, body=body)
        print("The response of LettersApi->detect_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LettersApi->detect_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**DetectAddress**](DetectAddress.md)

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

# **export_letter_history**
> ExportLetterHistory export_letter_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)

Export Letter History

_export letter history_

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
from clicksend.models.export_letter_history import ExportLetterHistory
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
    api_instance = clicksend.LettersApi(api_client)
    content_type = 'application/json' # str |  (optional)
    filename = 'Post_history.csv' # str |  (optional)
    q = 'q_example' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 50000 # int |  (optional)

    try:
        # Export Letter History
        api_response = api_instance.export_letter_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)
        print("The response of LettersApi->export_letter_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LettersApi->export_letter_history: %s\n" % e)
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

[**ExportLetterHistory**](ExportLetterHistory.md)

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

# **send_letter**
> SendLetter send_letter(content_type=content_type, send_letter_request=send_letter_request)

Send Letter

### Send letter

### **Supported File Types**

We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST https://rest.clicksend.com/v3/uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.

### **Letter Specification Guide**

Follow our [Letter specification guide](https://help.clicksend.com/article/wcpkkoou6c-post-letter-template) to ensure correct sending and letter template information.

### **Letter File Options**

### Use existing URL

With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.

When using an existing url make sure that it is publicly accessible as it will not work if it is private.

### Upload File to Our Server

With this option, you can use the [/uploads](/#upload-media-file) endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |
| template_used | integer(int1) | false | none | Whether using our letter template. Flag value must be 1 for yes or 0 for no. |
| duplex | integer(int1) | false | none | Whether letter is duplex. Flag value must be 1 for yes or 0 for no. |
| colour | integer(int1) | false | none | Whether letter is in colour. Flag value must be 1 for yes or 0 for no. |
| priority_post | integer(int1) | false | none | Whether letter is priority, Flag value must be 1 for yes or 0 for no. |
| source | string | false | none | Source being sent from |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_letter import SendLetter
from clicksend.models.send_letter_request import SendLetterRequest
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
    api_instance = clicksend.LettersApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_letter_request = clicksend.SendLetterRequest() # SendLetterRequest |  (optional)

    try:
        # Send Letter
        api_response = api_instance.send_letter(content_type=content_type, send_letter_request=send_letter_request)
        print("The response of LettersApi->send_letter:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LettersApi->send_letter: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_letter_request** | [**SendLetterRequest**](SendLetterRequest.md)|  | [optional] 

### Return type

[**SendLetter**](SendLetter.md)

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

# **view_letter_history**
> ViewLetterHistory view_letter_history(content_type=content_type)

View Letter History

_Get all letter history_

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
from clicksend.models.view_letter_history import ViewLetterHistory
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
    api_instance = clicksend.LettersApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Letter History
        api_response = api_instance.view_letter_history(content_type=content_type)
        print("The response of LettersApi->view_letter_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LettersApi->view_letter_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewLetterHistory**](ViewLetterHistory.md)

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

