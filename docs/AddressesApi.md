# clicksend.AddressesApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_return_address**](AddressesApi.md#create_return_address) | **POST** /v3/post/return-addresses | Create Return Address
[**delete_return_address**](AddressesApi.md#delete_return_address) | **DELETE** /v3/post/return-addresses/{return_address_id} | Delete Return Address
[**update_return_address**](AddressesApi.md#update_return_address) | **PUT** /v3/post/return-addresses/{return_address_id} | Update Return Address
[**view_specific_return_address**](AddressesApi.md#view_specific_return_address) | **GET** /v3/post/return-addresses/{return_address_id} | View Specific Return Address
[**view_your_return_addresses**](AddressesApi.md#view_your_return_addresses) | **GET** /v3/post/return-addresses | View Your Return Addresses


# **create_return_address**
> CreateReturnAddress create_return_address(content_type=content_type, create_return_address_request=create_return_address_request)

Create Return Address

_Create post return address_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| address_name | string | true | none | Your address name. |
| address_line_1 | string | true | none | Your address line 1 |
| address_city | string | true | none | Your city |
| address_postal_code | string | true | none | Your postal code |
| address_country | string | true | none | Your country |
| address_line_2 | string | false | none | Your address line 2 |
| address_state | string | false | none | Your state |


 Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


 <div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_return_address import CreateReturnAddress
from clicksend.models.create_return_address_request import CreateReturnAddressRequest
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
    api_instance = clicksend.AddressesApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_return_address_request = clicksend.CreateReturnAddressRequest() # CreateReturnAddressRequest |  (optional)

    try:
        # Create Return Address
        api_response = api_instance.create_return_address(content_type=content_type, create_return_address_request=create_return_address_request)
        print("The response of AddressesApi->create_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->create_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_return_address_request** | [**CreateReturnAddressRequest**](CreateReturnAddressRequest.md)|  | [optional] 

### Return type

[**CreateReturnAddress**](CreateReturnAddress.md)

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

# **delete_return_address**
> DeleteReturnAddress delete_return_address(return_address_id, content_type=content_type)

Delete Return Address

_Delete specific post return address_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| return_address_id | path | integer(int32) | true | Return address ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_return_address import DeleteReturnAddress
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
    api_instance = clicksend.AddressesApi(api_client)
    return_address_id = 'return_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Return Address
        api_response = api_instance.delete_return_address(return_address_id, content_type=content_type)
        print("The response of AddressesApi->delete_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->delete_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteReturnAddress**](DeleteReturnAddress.md)

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

# **update_return_address**
> UpdateReturnAddress update_return_address(return_address_id, content_type=content_type, update_return_address_request=update_return_address_request)

Update Return Address

_Update post return address_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| return_address_id | path | integer(int32) | true | Return address ID |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| address_name | string | true | none | Your address name. |
| address_line_1 | string | true | none | Your address line 1 |
| address_city | string | true | none | Your city |
| address_postal_code | string | true | none | Your postal code |
| address_country | string | true | none | Your country |
| address_line_2 | string | false | none | Your address line 2 |
| address_state | string | false | none | Your state |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_return_address import UpdateReturnAddress
from clicksend.models.update_return_address_request import UpdateReturnAddressRequest
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
    api_instance = clicksend.AddressesApi(api_client)
    return_address_id = 'return_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_return_address_request = clicksend.UpdateReturnAddressRequest() # UpdateReturnAddressRequest |  (optional)

    try:
        # Update Return Address
        api_response = api_instance.update_return_address(return_address_id, content_type=content_type, update_return_address_request=update_return_address_request)
        print("The response of AddressesApi->update_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->update_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_return_address_request** | [**UpdateReturnAddressRequest**](UpdateReturnAddressRequest.md)|  | [optional] 

### Return type

[**UpdateReturnAddress**](UpdateReturnAddress.md)

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

# **view_specific_return_address**
> ViewSpecificReturnAddress view_specific_return_address(return_address_id, content_type=content_type)

View Specific Return Address

_Get specific post return address_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| return_address_id | path | integer(int32) | true | Return address ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_return_address import ViewSpecificReturnAddress
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
    api_instance = clicksend.AddressesApi(api_client)
    return_address_id = 'return_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Return Address
        api_response = api_instance.view_specific_return_address(return_address_id, content_type=content_type)
        print("The response of AddressesApi->view_specific_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->view_specific_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificReturnAddress**](ViewSpecificReturnAddress.md)

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

# **view_your_return_addresses**
> ViewYourReturnAddresses view_your_return_addresses(content_type=content_type)

View Your Return Addresses

_Get list of post return addresses_

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
from clicksend.models.view_your_return_addresses import ViewYourReturnAddresses
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
    api_instance = clicksend.AddressesApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Your Return Addresses
        api_response = api_instance.view_your_return_addresses(content_type=content_type)
        print("The response of AddressesApi->view_your_return_addresses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->view_your_return_addresses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewYourReturnAddresses**](ViewYourReturnAddresses.md)

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

