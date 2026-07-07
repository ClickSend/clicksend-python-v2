# clicksend.TransactionsApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**current_payment_info**](TransactionsApi.md#current_payment_info) | **GET** /v3/recharge/credit-card | Current Payment Info
[**purchase_recharge_package**](TransactionsApi.md#purchase_recharge_package) | **PUT** /v3/recharge/purchase/{package_id} | Purchase Recharge Package
[**update_payment_info**](TransactionsApi.md#update_payment_info) | **PUT** /v3/recharge/credit-card | Update Payment Info
[**view_all_transactions**](TransactionsApi.md#view_all_transactions) | **GET** /v3/recharge/transactions | View All Transactions
[**view_recharge_packages**](TransactionsApi.md#view_recharge_packages) | **GET** /v3/recharge/packages | View Recharge Packages
[**view_specific_transaction**](TransactionsApi.md#view_specific_transaction) | **GET** /v3/recharge/transactions/{transaction_id} | View Specific Transaction


# **current_payment_info**
> CurrentPaymentInfo current_payment_info(content_type=content_type)

Current Payment Info

_Get current payment info_

This endpoint returns your current payment info, we do not store credit card numbers, only a card token for security reasons.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.current_payment_info import CurrentPaymentInfo
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
    api_instance = clicksend.TransactionsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Current Payment Info
        api_response = api_instance.current_payment_info(content_type=content_type)
        print("The response of TransactionsApi->current_payment_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TransactionsApi->current_payment_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**CurrentPaymentInfo**](CurrentPaymentInfo.md)

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

# **purchase_recharge_package**
> PurchaseRechargePackage purchase_recharge_package(package_id, content_type=content_type)

Purchase Recharge Package

_Purchase a package_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| package_id | path | integer(int32) | true | ID of package to purchase |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.purchase_recharge_package import PurchaseRechargePackage
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
    api_instance = clicksend.TransactionsApi(api_client)
    package_id = 'package_id_example' # str | 
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)

    try:
        # Purchase Recharge Package
        api_response = api_instance.purchase_recharge_package(package_id, content_type=content_type)
        print("The response of TransactionsApi->purchase_recharge_package:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TransactionsApi->purchase_recharge_package: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **package_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**PurchaseRechargePackage**](PurchaseRechargePackage.md)

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

# **update_payment_info**
> UpdatePaymentInfo update_payment_info(content_type=content_type, update_payment_info_request=update_payment_info_request)

Update Payment Info

_Update credit card info_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| number | string | true | none | Credit card number |
| expiry_month | integer(int32) | true | none | Expiry month of credit card |
| expiry_year | integer(int32) | true | none | Expiry year of credit card |
| cvc | integer(int32) | true | none | CVC number of credit card |
| name | string | true | none | Name printed on credit card |
| bank_name | string | true | none | Name of bank that credit card belongs to |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_payment_info import UpdatePaymentInfo
from clicksend.models.update_payment_info_request import UpdatePaymentInfoRequest
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
    api_instance = clicksend.TransactionsApi(api_client)
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    update_payment_info_request = clicksend.UpdatePaymentInfoRequest() # UpdatePaymentInfoRequest |  (optional)

    try:
        # Update Payment Info
        api_response = api_instance.update_payment_info(content_type=content_type, update_payment_info_request=update_payment_info_request)
        print("The response of TransactionsApi->update_payment_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TransactionsApi->update_payment_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **update_payment_info_request** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md)|  | [optional] 

### Return type

[**UpdatePaymentInfo**](UpdatePaymentInfo.md)

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

# **view_all_transactions**
> ViewAllTransactions view_all_transactions(content_type=content_type)

View All Transactions

_Purchase a package_

Get all transactions

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
from clicksend.models.view_all_transactions import ViewAllTransactions
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
    api_instance = clicksend.TransactionsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View All Transactions
        api_response = api_instance.view_all_transactions(content_type=content_type)
        print("The response of TransactionsApi->view_all_transactions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TransactionsApi->view_all_transactions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllTransactions**](ViewAllTransactions.md)

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

# **view_recharge_packages**
> ViewRechargePackages view_recharge_packages(content_type=content_type)

View Recharge Packages

_Get list of all packages_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| country | query | string | false | Two-letter country code ([ISO3166](https://en.wikipedia.org/wiki/ISO_3166)) |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_recharge_packages import ViewRechargePackages
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
    api_instance = clicksend.TransactionsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Recharge Packages
        api_response = api_instance.view_recharge_packages(content_type=content_type)
        print("The response of TransactionsApi->view_recharge_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TransactionsApi->view_recharge_packages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewRechargePackages**](ViewRechargePackages.md)

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

# **view_specific_transaction**
> ViewSpecificTransaction view_specific_transaction(transaction_id, content_type=content_type)

View Specific Transaction

_Get specific Transaction_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| transaction_id | path | string | true | ID of transaction to retrieve |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_transaction import ViewSpecificTransaction
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
    api_instance = clicksend.TransactionsApi(api_client)
    transaction_id = 'transaction_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Transaction
        api_response = api_instance.view_specific_transaction(transaction_id, content_type=content_type)
        print("The response of TransactionsApi->view_specific_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TransactionsApi->view_specific_transaction: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transaction_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificTransaction**](ViewSpecificTransaction.md)

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

