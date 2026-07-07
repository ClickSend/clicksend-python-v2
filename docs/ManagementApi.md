# clicksend.ManagementApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**view_account_details**](ManagementApi.md#view_account_details) | **GET** /v3/account | View Account Details
[**view_account_usage**](ManagementApi.md#view_account_usage) | **GET** /v3/account/usage/{year}/{month}/subaccount | View Account Usage


# **view_account_details**
> ViewAccountDetails view_account_details(content_type=content_type)

View Account Details

_Get account information_

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/#pagination" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_account_details import ViewAccountDetails
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
    api_instance = clicksend.ManagementApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Account Details
        api_response = api_instance.view_account_details(content_type=content_type)
        print("The response of ManagementApi->view_account_details:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ManagementApi->view_account_details: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAccountDetails**](ViewAccountDetails.md)

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

# **view_account_usage**
> ViewAccountUsage view_account_usage(year, month, content_type=content_type)

View Account Usage

_Get account usage_

| **Name** | **Type** | **Required** | **Restrictions** | **Description** |
| --- | --- | --- | --- | --- |
| year | string | true | none | Your account usage year. Example: 2019 |
| month | string | true | none | Your account usage month. Example: 4 |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/#pagination" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_account_usage import ViewAccountUsage
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
    api_instance = clicksend.ManagementApi(api_client)
    year = 'year_example' # str | 
    month = 'month_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Account Usage
        api_response = api_instance.view_account_usage(year, month, content_type=content_type)
        print("The response of ManagementApi->view_account_usage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ManagementApi->view_account_usage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **str**|  | 
 **month** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAccountUsage**](ViewAccountUsage.md)

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

