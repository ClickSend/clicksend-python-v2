# clicksend.SubaccountsOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_subaccount**](SubaccountsOtherApi.md#create_subaccount) | **POST** /v3/subaccounts | Create Subaccount
[**delete_subaccount**](SubaccountsOtherApi.md#delete_subaccount) | **DELETE** /v3/subaccounts/{subaccount_id} | Delete Subaccount
[**generate_new_api_key**](SubaccountsOtherApi.md#generate_new_api_key) | **PUT** /v3/subaccounts/{subaccount_id}/regen-api-key | Generate New API Key
[**update_subaccount**](SubaccountsOtherApi.md#update_subaccount) | **PUT** /v3/subaccounts/{subaccount_id} | Update Subaccount
[**view_specific_subaccount**](SubaccountsOtherApi.md#view_specific_subaccount) | **GET** /v3/subaccounts/{subaccount_id} | View Specific Subaccount
[**view_subaccounts**](SubaccountsOtherApi.md#view_subaccounts) | **GET** /v3/subaccounts | View Subaccounts


# **create_subaccount**
> CreateSubaccount create_subaccount(content_type=content_type, create_subaccount_request=create_subaccount_request)

Create Subaccount

_Create new subaccount_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| api_username | string | true | none | Your new api username. |
| password | string | true | none | Your new password |
| email | string | true | none | Your new email. |
| phone_number | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| first_name | string | true | none | Your firstname |
| last_name | string | true | none | Your lastname |
| access_users | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_billing | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_reporting | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_contacts | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_settings | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_subaccount import CreateSubaccount
from clicksend.models.create_subaccount_request import CreateSubaccountRequest
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
    api_instance = clicksend.SubaccountsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_subaccount_request = clicksend.CreateSubaccountRequest() # CreateSubaccountRequest |  (optional)

    try:
        # Create Subaccount
        api_response = api_instance.create_subaccount(content_type=content_type, create_subaccount_request=create_subaccount_request)
        print("The response of SubaccountsOtherApi->create_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubaccountsOtherApi->create_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_subaccount_request** | [**CreateSubaccountRequest**](CreateSubaccountRequest.md)|  | [optional] 

### Return type

[**CreateSubaccount**](CreateSubaccount.md)

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

# **delete_subaccount**
> DeleteSubaccount delete_subaccount(subaccount_id, content_type=content_type)

Delete Subaccount

_Delete a subaccount_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to delete |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_subaccount import DeleteSubaccount
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
    api_instance = clicksend.SubaccountsOtherApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Subaccount
        api_response = api_instance.delete_subaccount(subaccount_id, content_type=content_type)
        print("The response of SubaccountsOtherApi->delete_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubaccountsOtherApi->delete_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteSubaccount**](DeleteSubaccount.md)

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

# **generate_new_api_key**
> GenerateNewApiKey generate_new_api_key(subaccount_id, content_type=content_type, generate_new_api_key_request=generate_new_api_key_request)

Generate New API Key

_Regenerate an API Key_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to regenerate API key for |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.generate_new_api_key import GenerateNewApiKey
from clicksend.models.generate_new_api_key_request import GenerateNewApiKeyRequest
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
    api_instance = clicksend.SubaccountsOtherApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    generate_new_api_key_request = clicksend.GenerateNewApiKeyRequest() # GenerateNewApiKeyRequest |  (optional)

    try:
        # Generate New API Key
        api_response = api_instance.generate_new_api_key(subaccount_id, content_type=content_type, generate_new_api_key_request=generate_new_api_key_request)
        print("The response of SubaccountsOtherApi->generate_new_api_key:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubaccountsOtherApi->generate_new_api_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **generate_new_api_key_request** | [**GenerateNewApiKeyRequest**](GenerateNewApiKeyRequest.md)|  | [optional] 

### Return type

[**GenerateNewApiKey**](GenerateNewApiKey.md)

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

# **update_subaccount**
> UpdateSubaccount update_subaccount(subaccount_id, content_type=content_type, update_subaccount_request=update_subaccount_request)

Update Subaccount

_Update subaccount_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to update |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| api_username | string | true | none | Your new api username. |
| password | string | true | none | Your new password |
| email | string | true | none | Your new email. |
| phone_number | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| first_name | string | true | none | Your firstname |
| last_name | string | true | none | Your lastname |
| access_users | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_billing | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_reporting | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_contacts | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_settings | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_subaccount import UpdateSubaccount
from clicksend.models.update_subaccount_request import UpdateSubaccountRequest
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
    api_instance = clicksend.SubaccountsOtherApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_subaccount_request = clicksend.UpdateSubaccountRequest() # UpdateSubaccountRequest |  (optional)

    try:
        # Update Subaccount
        api_response = api_instance.update_subaccount(subaccount_id, content_type=content_type, update_subaccount_request=update_subaccount_request)
        print("The response of SubaccountsOtherApi->update_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubaccountsOtherApi->update_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_subaccount_request** | [**UpdateSubaccountRequest**](UpdateSubaccountRequest.md)|  | [optional] 

### Return type

[**UpdateSubaccount**](UpdateSubaccount.md)

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

# **view_specific_subaccount**
> ViewSpecificSubaccount view_specific_subaccount(subaccount_id, content_type=content_type)

View Specific Subaccount

_Get specific subaccount_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to get |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_subaccount import ViewSpecificSubaccount
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
    api_instance = clicksend.SubaccountsOtherApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Subaccount
        api_response = api_instance.view_specific_subaccount(subaccount_id, content_type=content_type)
        print("The response of SubaccountsOtherApi->view_specific_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubaccountsOtherApi->view_specific_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificSubaccount**](ViewSpecificSubaccount.md)

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

# **view_subaccounts**
> ViewSubaccounts view_subaccounts(content_type=content_type)

View Subaccounts

_Get all subaccounts_

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
from clicksend.models.view_subaccounts import ViewSubaccounts
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
    api_instance = clicksend.SubaccountsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Subaccounts
        api_response = api_instance.view_subaccounts(content_type=content_type)
        print("The response of SubaccountsOtherApi->view_subaccounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubaccountsOtherApi->view_subaccounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSubaccounts**](ViewSubaccounts.md)

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

