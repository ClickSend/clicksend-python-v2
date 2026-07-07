# clicksend.OwnNumbersApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_own_number**](OwnNumbersApi.md#delete_own_number) | **DELETE** /v3/own-numbers/{own_number_id} | Delete Own Number
[**get_own_number_detail**](OwnNumbersApi.md#get_own_number_detail) | **GET** /v3/own-numbers/{own_number_id} | Get Own Number Detail
[**list_own_numbers**](OwnNumbersApi.md#list_own_numbers) | **GET** /v3/own-numbers | List Own Numbers
[**request_own_number_verification_otp**](OwnNumbersApi.md#request_own_number_verification_otp) | **POST** /v3/own-numbers/verifications | Request Own Number Verification OTP
[**update_own_number**](OwnNumbersApi.md#update_own_number) | **PATCH** /v3/own-numbers/{own_number_id} | Update Own Number
[**verify_own_number_otp**](OwnNumbersApi.md#verify_own_number_otp) | **POST** /v3/own-numbers/verifications/{verification_id}/verify | Verify Own Number OTP


# **delete_own_number**
> OwnNumber delete_own_number(own_number_id, content_type=content_type)

Delete Own Number

_Delete a specific own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| own_number_id | path | uuid | true | ID of the own number |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.own_number import OwnNumber
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
    api_instance = clicksend.OwnNumbersApi(api_client)
    own_number_id = 'own_number_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Own Number
        api_response = api_instance.delete_own_number(own_number_id, content_type=content_type)
        print("The response of OwnNumbersApi->delete_own_number:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OwnNumbersApi->delete_own_number: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **own_number_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**OwnNumber**](OwnNumber.md)

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

# **get_own_number_detail**
> OwnNumber get_own_number_detail(own_number_id, content_type=content_type)

Get Own Number Detail

_Get a specific own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| own_number_id | path | uuid | true | ID of the own number |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.own_number import OwnNumber
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
    api_instance = clicksend.OwnNumbersApi(api_client)
    own_number_id = 'own_number_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Own Number Detail
        api_response = api_instance.get_own_number_detail(own_number_id, content_type=content_type)
        print("The response of OwnNumbersApi->get_own_number_detail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OwnNumbersApi->get_own_number_detail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **own_number_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**OwnNumber**](OwnNumber.md)

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

# **list_own_numbers**
> ListOwnNumbers list_own_numbers(content_type=content_type)

List Own Numbers

_List own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| offset | query | uuid | false | Page(offset) to be used for pagination. Example: `offset=f99872cc-11a6-48ba-a9f2-bcfb6dd1e3d4#8fa5ebc2-777b-45db-a448-ec76a40d4384` |
| page_size | query | integer | false | Number of records per page. Default: 10. Range \[1..500\] |
| filter\[status\]\[\] | query | string | false | Filter by statuses. Value must be in enum \[`PENDING`, `APPROVED`, `REJECTED`\]. For example: `filter[status][0]=PENDING&filter[status][1]=APPROVED` . |
| sort_by | query | string | false | Sort by parameter. Default: `created_timestamp` |
| sort_direction | query | string | false | Direction of sorting. Default: `asc`. Value must be in enum \[`asc`, `desc`\]. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

 This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_own_numbers import ListOwnNumbers
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
    api_instance = clicksend.OwnNumbersApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # List Own Numbers
        api_response = api_instance.list_own_numbers(content_type=content_type)
        print("The response of OwnNumbersApi->list_own_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OwnNumbersApi->list_own_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ListOwnNumbers**](ListOwnNumbers.md)

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

# **request_own_number_verification_otp**
> RequestOwnNumberVerificationOtp request_own_number_verification_otp(content_type=content_type, request_own_number_verification_otp_request=request_own_number_verification_otp_request)

Request Own Number Verification OTP

_Request to generate own number verification OTP_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| label | string | false | none | Custom label for phone number. Length must be between 1 - 200 characters. |
| phone_number | string | true | none | Phone number. |
| country | string | false | none | Country code. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.request_own_number_verification_otp import RequestOwnNumberVerificationOtp
from clicksend.models.request_own_number_verification_otp_request import RequestOwnNumberVerificationOtpRequest
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
    api_instance = clicksend.OwnNumbersApi(api_client)
    content_type = 'application/json' # str |  (optional)
    request_own_number_verification_otp_request = clicksend.RequestOwnNumberVerificationOtpRequest() # RequestOwnNumberVerificationOtpRequest |  (optional)

    try:
        # Request Own Number Verification OTP
        api_response = api_instance.request_own_number_verification_otp(content_type=content_type, request_own_number_verification_otp_request=request_own_number_verification_otp_request)
        print("The response of OwnNumbersApi->request_own_number_verification_otp:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OwnNumbersApi->request_own_number_verification_otp: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **request_own_number_verification_otp_request** | [**RequestOwnNumberVerificationOtpRequest**](RequestOwnNumberVerificationOtpRequest.md)|  | [optional] 

### Return type

[**RequestOwnNumberVerificationOtp**](RequestOwnNumberVerificationOtp.md)

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

# **update_own_number**
> OwnNumber update_own_number(own_number_id)

Update Own Number

_Update details of a specific own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| own_number_id | path | uuid | true | ID of the own number |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| label | string | false | none | Custom label for phone number. Length must be between 1 - 200 characters. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example


```python
import clicksend
from clicksend.models.own_number import OwnNumber
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
    api_instance = clicksend.OwnNumbersApi(api_client)
    own_number_id = 'own_number_id_example' # str | 

    try:
        # Update Own Number
        api_response = api_instance.update_own_number(own_number_id)
        print("The response of OwnNumbersApi->update_own_number:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OwnNumbersApi->update_own_number: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **own_number_id** | **str**|  | 

### Return type

[**OwnNumber**](OwnNumber.md)

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

# **verify_own_number_otp**
> VerifyOwnNumberOtp verify_own_number_otp(verification_id, content_type=content_type, verify_own_number_otp_request=verify_own_number_otp_request)

Verify Own Number OTP

_Request to verify an OTP for Own Number verification_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| verification_id | path | uuid | true | ID of the Own Number verification |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| code | string | true | none | OTP code. Length must be 6 characters |
| phone_number | string | true | none | Phone number. |
| country | string | false | none | Country code. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.verify_own_number_otp import VerifyOwnNumberOtp
from clicksend.models.verify_own_number_otp_request import VerifyOwnNumberOtpRequest
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
    api_instance = clicksend.OwnNumbersApi(api_client)
    verification_id = 'verification_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    verify_own_number_otp_request = clicksend.VerifyOwnNumberOtpRequest() # VerifyOwnNumberOtpRequest |  (optional)

    try:
        # Verify Own Number OTP
        api_response = api_instance.verify_own_number_otp(verification_id, content_type=content_type, verify_own_number_otp_request=verify_own_number_otp_request)
        print("The response of OwnNumbersApi->verify_own_number_otp:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OwnNumbersApi->verify_own_number_otp: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **verification_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **verify_own_number_otp_request** | [**VerifyOwnNumberOtpRequest**](VerifyOwnNumberOtpRequest.md)|  | [optional] 

### Return type

[**VerifyOwnNumberOtp**](VerifyOwnNumberOtp.md)

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

