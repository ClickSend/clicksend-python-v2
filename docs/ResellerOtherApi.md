# clicksend.ResellerOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_reseller_account**](ResellerOtherApi.md#create_reseller_account) | **POST** /v3/reseller/accounts | Create Reseller Account
[**reseller_transfer_credit**](ResellerOtherApi.md#reseller_transfer_credit) | **PUT** /v3/reseller/transfer-credit | Reseller Transfer Credit
[**update_client_account**](ResellerOtherApi.md#update_client_account) | **PUT** /v3/reseller/accounts/{client_user_id} | Update Client Account
[**view_client_accounts**](ResellerOtherApi.md#view_client_accounts) | **GET** /v3/reseller/accounts | View Client Accounts
[**view_specific_client_account**](ResellerOtherApi.md#view_specific_client_account) | **GET** /v3/reseller/accounts/{client_user_id} | View Specific Client Account


# **create_reseller_account**
> CreateResellerAccount create_reseller_account(content_type=content_type, create_reseller_account_request=create_reseller_account_request)

Create Reseller Account

_Create reseller account_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| username | string | true | none | Account username |
| password | string | true | none | Account password (unhashed) |
| user_email | string | true | none | Account email |
| user_phone | string | true | none | Account phone number |
| user_first_name | string | true | none | Account owner first name |
| user_last_name | string | true | none | Account owner last name |
| account_name | string | true | none | Account name (usually company name) |
| country | string | true | none | Country of account holder |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_reseller_account import CreateResellerAccount
from clicksend.models.create_reseller_account_request import CreateResellerAccountRequest
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
    api_instance = clicksend.ResellerOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_reseller_account_request = clicksend.CreateResellerAccountRequest() # CreateResellerAccountRequest |  (optional)

    try:
        # Create Reseller Account
        api_response = api_instance.create_reseller_account(content_type=content_type, create_reseller_account_request=create_reseller_account_request)
        print("The response of ResellerOtherApi->create_reseller_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResellerOtherApi->create_reseller_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_reseller_account_request** | [**CreateResellerAccountRequest**](CreateResellerAccountRequest.md)|  | [optional] 

### Return type

[**CreateResellerAccount**](CreateResellerAccount.md)

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

# **reseller_transfer_credit**
> ResellerTransferCredit reseller_transfer_credit(content_type=content_type, update_payment_info_request=update_payment_info_request)

Reseller Transfer Credit

_Transfer Credit_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| client_user_id | integer(int32) | true | none | User ID of client |
| balance | integer(int32) | true | none | Balance to transfer |
| currency | string | true | none | Currency of balance to transfer |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.reseller_transfer_credit import ResellerTransferCredit
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
    api_instance = clicksend.ResellerOtherApi(api_client)
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    update_payment_info_request = clicksend.UpdatePaymentInfoRequest() # UpdatePaymentInfoRequest |  (optional)

    try:
        # Reseller Transfer Credit
        api_response = api_instance.reseller_transfer_credit(content_type=content_type, update_payment_info_request=update_payment_info_request)
        print("The response of ResellerOtherApi->reseller_transfer_credit:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResellerOtherApi->reseller_transfer_credit: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **update_payment_info_request** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md)|  | [optional] 

### Return type

[**ResellerTransferCredit**](ResellerTransferCredit.md)

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

# **update_client_account**
> UpdateClientAccount update_client_account(client_user_id, content_type=content_type, update_payment_info_request=update_payment_info_request)

Update Client Account

_Update Reseller clients Account_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| client_user_id | path | integer(int32) | true | User ID of client |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| username | string | true | none | Account username |
| password | string | true | none | Account password (unhashed) |
| user_email | string | true | none | Account email |
| user_phone | string | true | none | Account phone number |
| user_first_name | string | true | none | Account owner first name |
| user_last_name | string | true | none | Account owner last name |
| account_name | string | true | none | Account name (usually company name) |
| country | string | true | none | Country of account holder |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_client_account import UpdateClientAccount
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
    api_instance = clicksend.ResellerOtherApi(api_client)
    client_user_id = 'client_user_id_example' # str | 
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    update_payment_info_request = clicksend.UpdatePaymentInfoRequest() # UpdatePaymentInfoRequest |  (optional)

    try:
        # Update Client Account
        api_response = api_instance.update_client_account(client_user_id, content_type=content_type, update_payment_info_request=update_payment_info_request)
        print("The response of ResellerOtherApi->update_client_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResellerOtherApi->update_client_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client_user_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_payment_info_request** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md)|  | [optional] 

### Return type

[**UpdateClientAccount**](UpdateClientAccount.md)

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

# **view_client_accounts**
> ViewClientAccounts view_client_accounts(content_type=content_type)

View Client Accounts

_Get list of reseller accounts_

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
from clicksend.models.view_client_accounts import ViewClientAccounts
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
    api_instance = clicksend.ResellerOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Client Accounts
        api_response = api_instance.view_client_accounts(content_type=content_type)
        print("The response of ResellerOtherApi->view_client_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResellerOtherApi->view_client_accounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewClientAccounts**](ViewClientAccounts.md)

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

# **view_specific_client_account**
> ViewSpecificClientAccount view_specific_client_account(client_user_id, content_type=content_type)

View Specific Client Account

_Get Reseller clients Account_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| client_user_id | path | integer(int32) | true | User ID of client |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_client_account import ViewSpecificClientAccount
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
    api_instance = clicksend.ResellerOtherApi(api_client)
    client_user_id = 'client_user_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Client Account
        api_response = api_instance.view_specific_client_account(client_user_id, content_type=content_type)
        print("The response of ResellerOtherApi->view_specific_client_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResellerOtherApi->view_specific_client_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client_user_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificClientAccount**](ViewSpecificClientAccount.md)

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

