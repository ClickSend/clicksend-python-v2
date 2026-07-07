# clicksend.MmsOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_mms_price**](MmsOtherApi.md#calculate_mms_price) | **POST** /v3/mms/price | Calculate MMS Price
[**export_mms_history**](MmsOtherApi.md#export_mms_history) | **GET** /v3/mms/history/export | Export MMS History
[**send_mms**](MmsOtherApi.md#send_mms) | **POST** /v3/mms/send | Send MMS
[**view_mms_history**](MmsOtherApi.md#view_mms_history) | **GET** /v3/mms/history | View MMS History


# **calculate_mms_price**
> CalculateMmsPrice calculate_mms_price(content_type=content_type, calculate_mms_price_request=calculate_mms_price_request)

Calculate MMS Price

_Get Price for MMS sent_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| media_file | string | true | none | Media file you want to send |
| to | string | true | none | Recipient phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format |
| body | string | true | none | Your message |
| subject | string | true | none | Subject line (max 20 characters) |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_mms_price import CalculateMmsPrice
from clicksend.models.calculate_mms_price_request import CalculateMmsPriceRequest
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
    api_instance = clicksend.MmsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_mms_price_request = clicksend.CalculateMmsPriceRequest() # CalculateMmsPriceRequest |  (optional)

    try:
        # Calculate MMS Price
        api_response = api_instance.calculate_mms_price(content_type=content_type, calculate_mms_price_request=calculate_mms_price_request)
        print("The response of MmsOtherApi->calculate_mms_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsOtherApi->calculate_mms_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_mms_price_request** | [**CalculateMmsPriceRequest**](CalculateMmsPriceRequest.md)|  | [optional] 

### Return type

[**CalculateMmsPrice**](CalculateMmsPrice.md)

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

# **export_mms_history**
> ExportMmsHistory export_mms_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)

Export MMS History

_Export all mms history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to download history as |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_mms_history import ExportMmsHistory
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
    api_instance = clicksend.MmsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    filename = 'MMS_history.csv' # str |  (optional)
    q = 'q_example' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 50000 # int |  (optional)

    try:
        # Export MMS History
        api_response = api_instance.export_mms_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)
        print("The response of MmsOtherApi->export_mms_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsOtherApi->export_mms_history: %s\n" % e)
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

[**ExportMmsHistory**](ExportMmsHistory.md)

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

# **send_mms**
> SendMms send_mms(content_type=content_type, send_mms_request=send_mms_request)

Send MMS

_Send MMS_

You can post **up to 1000 messages** with each API call. You can send to a mix of contacts and contact lists, as long as the total number of recipients is up to 1000. The response contains a status and details for each recipient.

Refer to [<b>Application Status Codes</b>](/#application-status-codes) for the possible response message status strings.

### **How many characters can I send in a message?**

### Standard MMS Message

1500 characters

### Unicode MMS Message

500 characters

If a message is longer the allowed number of characters it will be truncated. If a message contains any characters that aren't in the GSM 03.38 character set, the message type will be treated as unicode. ([https://en.wikipedia.org/wiki/GSM_03.38](https://en.wikipedia.org/wiki/GSM_03.38))

### Maximum File Size

You can send a single attachment with a size of up to 250 kB. Some older devices can only accept attachments with up to 30 kB.

### Supported File Types

- Supported file types are listed below. If you need to convert a file to a supported format, it can be first passed to our uploads endpoint: `/uploads?convert=mms`
- This will return a URL to the converted image file that can be used in the /mms/send endpoint.
- Contact us to add support for any other file type.
    

### Images

| File type | Required to be passed to uploads endpoint first? |
| --- | --- |
| `jpg` | No |
| `gif` | No |
| `jpeg` | Yes |
| `png` | Yes |
| `bmp` | Yes |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| media_file | string | true | none | Media file you want to send |
| to | string | true | none | Recipient phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format |
| body | string | true | none | Your message |
| subject | string | true | none | Subject line (max 20 characters) |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_mms import SendMms
from clicksend.models.send_mms_request import SendMmsRequest
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
    api_instance = clicksend.MmsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_mms_request = clicksend.SendMmsRequest() # SendMmsRequest |  (optional)

    try:
        # Send MMS
        api_response = api_instance.send_mms(content_type=content_type, send_mms_request=send_mms_request)
        print("The response of MmsOtherApi->send_mms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsOtherApi->send_mms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_mms_request** | [**SendMmsRequest**](SendMmsRequest.md)|  | [optional] 

### Return type

[**SendMms**](SendMms.md)

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

# **view_mms_history**
> ViewMmsHistory view_mms_history(content_type=content_type, limit=limit)

View MMS History

_Get all mms history_

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
from clicksend.models.view_mms_history import ViewMmsHistory
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
    api_instance = clicksend.MmsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    limit = 100 # int |  (optional)

    try:
        # View MMS History
        api_response = api_instance.view_mms_history(content_type=content_type, limit=limit)
        print("The response of MmsOtherApi->view_mms_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsOtherApi->view_mms_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 

### Return type

[**ViewMmsHistory**](ViewMmsHistory.md)

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

