# clicksend.PostcardsApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_postcard_price**](PostcardsApi.md#calculate_postcard_price) | **POST** /v3/post/postcards/price | Calculate Postcard Price
[**cancel_scheduled_postcard**](PostcardsApi.md#cancel_scheduled_postcard) | **PUT** /v3/post/postcards/{message_id}/cancel | Cancel Scheduled Postcard
[**export_postcard_history**](PostcardsApi.md#export_postcard_history) | **GET** /v3/post/postcards/history/export | Export Postcard History
[**send_postcard**](PostcardsApi.md#send_postcard) | **POST** /v3/post/postcards/send | Send Postcard
[**view_postcard_history**](PostcardsApi.md#view_postcard_history) | **GET** /v3/post/postcards/history | View Postcard History


# **calculate_postcard_price**
> CalculatePostcardPrice calculate_postcard_price(content_type=content_type, send_postcard_request=send_postcard_request)

Calculate Postcard Price

_Calculate price for sending one or more postcards_

For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.

- Supply a single pdf with 2 pages (front and back)
- Supply 2 urls to seperate PDFs
    

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_urls | \[string\] | true | none | Postcard file URLs |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_postcard_price import CalculatePostcardPrice
from clicksend.models.send_postcard_request import SendPostcardRequest
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
    api_instance = clicksend.PostcardsApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_postcard_request = clicksend.SendPostcardRequest() # SendPostcardRequest |  (optional)

    try:
        # Calculate Postcard Price
        api_response = api_instance.calculate_postcard_price(content_type=content_type, send_postcard_request=send_postcard_request)
        print("The response of PostcardsApi->calculate_postcard_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostcardsApi->calculate_postcard_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_postcard_request** | [**SendPostcardRequest**](SendPostcardRequest.md)|  | [optional] 

### Return type

[**CalculatePostcardPrice**](CalculatePostcardPrice.md)

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

# **cancel_scheduled_postcard**
> CancelScheduledPostcard cancel_scheduled_postcard(message_id)

Cancel Scheduled Postcard

_Cancel scheduled postcard_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | query | string | true | Message ID of the scheduled postcard that is to be cancelled. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example


```python
import clicksend
from clicksend.models.cancel_scheduled_postcard import CancelScheduledPostcard
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
    api_instance = clicksend.PostcardsApi(api_client)
    message_id = 'message_id_example' # str | 

    try:
        # Cancel Scheduled Postcard
        api_response = api_instance.cancel_scheduled_postcard(message_id)
        print("The response of PostcardsApi->cancel_scheduled_postcard:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostcardsApi->cancel_scheduled_postcard: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 

### Return type

[**CancelScheduledPostcard**](CancelScheduledPostcard.md)

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

# **export_postcard_history**
> ExportPostcardHistory export_postcard_history(content_type=content_type)

Export Postcard History

_Export postcard history to a CSV file_

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
from clicksend.models.export_postcard_history import ExportPostcardHistory
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
    api_instance = clicksend.PostcardsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Export Postcard History
        api_response = api_instance.export_postcard_history(content_type=content_type)
        print("The response of PostcardsApi->export_postcard_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostcardsApi->export_postcard_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ExportPostcardHistory**](ExportPostcardHistory.md)

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

# **send_postcard**
> SendPostcard send_postcard(content_type=content_type, send_postcard_request=send_postcard_request)

Send Postcard

_Send one or more postcards_

### **Supported File Types**

We support PDF, docx, doc, jpg, gif, png, and bmp. Contact us to add support for any other file type. If you're using docx, doc, jpg, gif, png, or bmp files, you'll need to convert the file first using our uploads endpoint with the querystring parameter ?convert=postcard. e.g. POST /uploads?convert=postcard. This will return a URL to the converted pdf file that can be used in the /post/postcards/send endpoint.

### **Postcard Specification Guide**

Follow our [Postcard specification guide](https://help.clicksend.com/article/ysyql7bsr1-postcard-template) to ensure correct sending and postcard template information.

### **Postcard File Options**

### Use existing URL

With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.

When using an existing url make sure that it is publicly accessible as it will not work if it is private.

For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.

- Supply a single pdf with 2 pages (front and back)
- Supply 2 urls to seperate PDFs
    

### Upload File to Our Server

With this option, you can use the [/uploads](/#upload-media-file) endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/postcards/send` endpoint.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_urls | \[string\] | true | none | Postcard file URLs |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_postcard import SendPostcard
from clicksend.models.send_postcard_request import SendPostcardRequest
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
    api_instance = clicksend.PostcardsApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_postcard_request = clicksend.SendPostcardRequest() # SendPostcardRequest |  (optional)

    try:
        # Send Postcard
        api_response = api_instance.send_postcard(content_type=content_type, send_postcard_request=send_postcard_request)
        print("The response of PostcardsApi->send_postcard:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostcardsApi->send_postcard: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_postcard_request** | [**SendPostcardRequest**](SendPostcardRequest.md)|  | [optional] 

### Return type

[**SendPostcard**](SendPostcard.md)

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

# **view_postcard_history**
> ViewPostcardHistory view_postcard_history(content_type=content_type)

View Postcard History

_Retrieve the history of postcards sent or scheduled_

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
from clicksend.models.view_postcard_history import ViewPostcardHistory
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
    api_instance = clicksend.PostcardsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Postcard History
        api_response = api_instance.view_postcard_history(content_type=content_type)
        print("The response of PostcardsApi->view_postcard_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostcardsApi->view_postcard_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewPostcardHistory**](ViewPostcardHistory.md)

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

