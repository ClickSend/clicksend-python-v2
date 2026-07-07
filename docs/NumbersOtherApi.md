# clicksend.NumbersOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**purchase_dedicated_number**](NumbersOtherApi.md#purchase_dedicated_number) | **POST** /v3/numbers/buy/{dedicated_number} | Purchase Dedicated Number
[**register_numbers**](NumbersOtherApi.md#register_numbers) | **POST** /v3/numbers/registrations/number-types/{number_type}/country/{country_code} | Register Numbers
[**view_available_numbers**](NumbersOtherApi.md#view_available_numbers) | **GET** /v3/numbers/search/{country} | View Available Numbers
[**view_your_numbers**](NumbersOtherApi.md#view_your_numbers) | **GET** /v3/numbers | View Your Numbers


# **purchase_dedicated_number**
> PurchaseDedicatedNumber purchase_dedicated_number(dedicated_number, buy_number_request, content_type=content_type, type=type)

Purchase Dedicated Number

_Buy dedicated number_

This endpoint allows you to purchase a dedicated phone number for messaging services. You can optionally include registration data for compliance purposes.

### Request Body

| Field | Type | Required | Description |
| --- | --- | --- | --- |
| dedicated_number | string | true | Phone number to purchase |
| type | string | true | Service type (sms, mms) |
| registration_data | object | false | Registration data for compliance (AU SMS/MMS numbers only) |

#### Registration Data Fields (Optional)

| Field | Type | Required | Description |
| --- | --- | --- | --- |
| business_name | string | true | Name of the business (2 - 100 characters) |
| business_address | string | true | Business address (5 - 150 characters) |
| suburb | string | true | Suburb/City (2 - 50 characters) |
| postcode | string | true | Postal code (2 - 20 characters) |
| state | string | true | State/Province (2 - 50 characters) |
| contact_name | string | true | Contact person name (2 - 100 characters) |
| contact_number | string | true | Contact phone number (valid local or international phone number) |
| country | string | true | Country code (ISO 3166-1 alpha-2) |


### Path Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | path | string | true | Phone number to purchase |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.buy_number_request import BuyNumberRequest
from clicksend.models.purchase_dedicated_number import PurchaseDedicatedNumber
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
    api_instance = clicksend.NumbersOtherApi(api_client)
    dedicated_number = '+614197651956' # str | Phone number to purchase
    buy_number_request = clicksend.BuyNumberRequest() # BuyNumberRequest | 
    content_type = 'application/json' # str |  (optional)
    type = 'sms' # str |  (optional)

    try:
        # Purchase Dedicated Number
        api_response = api_instance.purchase_dedicated_number(dedicated_number, buy_number_request, content_type=content_type, type=type)
        print("The response of NumbersOtherApi->purchase_dedicated_number:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumbersOtherApi->purchase_dedicated_number: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dedicated_number** | **str**| Phone number to purchase | 
 **buy_number_request** | [**BuyNumberRequest**](BuyNumberRequest.md)|  | 
 **content_type** | **str**|  | [optional] 
 **type** | **str**|  | [optional] 

### Return type

[**PurchaseDedicatedNumber**](PurchaseDedicatedNumber.md)

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

# **register_numbers**
> RegisterNumbers register_numbers(number_type, country_code, content_type=content_type, register_numbers_request=register_numbers_request)

Register Numbers

<div style="background-color: #e8f4ff; padding: 15px; border-radius: 4px; border-left: 4px solid #0066cc;">
This endpoint is currently only available for <b>Canada 10DLC</b> number registration.
</div>

Registers a number that requires additional verification information. This endpoint facilitates the registration process for numbers requiring special compliance documentation.

After submission, ClickSend's compliance team will review the registration and notify you of the approval status.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.
<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.register_numbers import RegisterNumbers
from clicksend.models.register_numbers_request import RegisterNumbersRequest
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
    api_instance = clicksend.NumbersOtherApi(api_client)
    number_type = '10dlc' # str | The type of number being registered
    country_code = 'US, CA' # str | Two-character ISO country code
    content_type = 'application/json' # str |  (optional)
    register_numbers_request = clicksend.RegisterNumbersRequest() # RegisterNumbersRequest |  (optional)

    try:
        # Register Numbers
        api_response = api_instance.register_numbers(number_type, country_code, content_type=content_type, register_numbers_request=register_numbers_request)
        print("The response of NumbersOtherApi->register_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumbersOtherApi->register_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **number_type** | **str**| The type of number being registered | 
 **country_code** | **str**| Two-character ISO country code | 
 **content_type** | **str**|  | [optional] 
 **register_numbers_request** | [**RegisterNumbersRequest**](RegisterNumbersRequest.md)|  | [optional] 

### Return type

[**RegisterNumbers**](RegisterNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_available_numbers**
> ViewAvailableNumbers view_available_numbers(country, content_type=content_type)

View Available Numbers

_Get all dedicated numbers by country_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| country | path | string | true | Country code to search |
| search | query | string | false | Your search pattern or query. |
| search_type | query | integer(int32) | false | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |
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
from clicksend.models.view_available_numbers import ViewAvailableNumbers
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
    api_instance = clicksend.NumbersOtherApi(api_client)
    country = 'country_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Available Numbers
        api_response = api_instance.view_available_numbers(country, content_type=content_type)
        print("The response of NumbersOtherApi->view_available_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumbersOtherApi->view_available_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAvailableNumbers**](ViewAvailableNumbers.md)

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

# **view_your_numbers**
> ViewYourNumbers view_your_numbers(content_type=content_type, page=page, limit=limit, q=q, q2=q2, excluding_number_type=excluding_number_type, exclude_10dlc_campaign=exclude_10dlc_campaign)

View Your Numbers

_Get all available dedicated numbers_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |
| q | query | string | false | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: `type`, `number_type`, `country` |
| q2 | query | string | false | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: `type` |
| excluding_number_type | query | string | false | Exclude specific number types from the results. Available number types: `shortcode`, `tollfree`, `10DLC` |
| exclude_10dlc_campaign | query | boolean | false | When set to true, excludes all numbers that are associated with 10DLC campaigns |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_your_numbers import ViewYourNumbers
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
    api_instance = clicksend.NumbersOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | Page number (optional) (default to 1)
    limit = 15 # int | Number of records per page (optional) (default to 15)
    q = 'type:sms,number_type:longcode,country:AU' # str | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: - `type`: Message type (e.g., `SMS`, `MMS`) - `number_type`: Number classification (e.g., `longcode`, `shortcode`, `tollfree`, `10DLC`) - `country`: Two-letter country code (e.g., `AU`, `US`)  (optional)
    q2 = 'type:mms' # str |  (optional)
    excluding_number_type = '10DLC' # str | Exclude specific number types from the results. Available number types: - `shortcode` - `tollfree` - `10DLC`  (optional)
    exclude_10dlc_campaign = False # bool | When set to true, excludes all numbers that are associated with 10DLC campaigns (optional) (default to False)

    try:
        # View Your Numbers
        api_response = api_instance.view_your_numbers(content_type=content_type, page=page, limit=limit, q=q, q2=q2, excluding_number_type=excluding_number_type, exclude_10dlc_campaign=exclude_10dlc_campaign)
        print("The response of NumbersOtherApi->view_your_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NumbersOtherApi->view_your_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| Page number | [optional] [default to 1]
 **limit** | **int**| Number of records per page | [optional] [default to 15]
 **q** | **str**| Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: - &#x60;type&#x60;: Message type (e.g., &#x60;SMS&#x60;, &#x60;MMS&#x60;) - &#x60;number_type&#x60;: Number classification (e.g., &#x60;longcode&#x60;, &#x60;shortcode&#x60;, &#x60;tollfree&#x60;, &#x60;10DLC&#x60;) - &#x60;country&#x60;: Two-letter country code (e.g., &#x60;AU&#x60;, &#x60;US&#x60;)  | [optional] 
 **q2** | **str**|  | [optional] 
 **excluding_number_type** | **str**| Exclude specific number types from the results. Available number types: - &#x60;shortcode&#x60; - &#x60;tollfree&#x60; - &#x60;10DLC&#x60;  | [optional] 
 **exclude_10dlc_campaign** | **bool**| When set to true, excludes all numbers that are associated with 10DLC campaigns | [optional] [default to False]

### Return type

[**ViewYourNumbers**](ViewYourNumbers.md)

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

