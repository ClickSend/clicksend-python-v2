# clicksend.VerificationOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**forgot_password**](VerificationOtherApi.md#forgot_password) | **PUT** /v3/forgot-password | Forgot Password
[**forgot_username**](VerificationOtherApi.md#forgot_username) | **PUT** /v3/forgot-username | Forgot Username


# **forgot_password**
> ForgotPassword forgot_password(content_type=content_type, forgot_password_request=forgot_password_request)

Forgot Password

_Forgot password_

A user can send their username to this endpoint to be sent an email with their registered email address that will have a verification code.

Once you have this verification email containing the code you can send it to the [forgotten-password/verify](/#verify-forgot-password) endpoint along with a new password and the ID of that subaccount.

_Ask your administrator if you do not know your subaccount id._

### Properties

| **Name** | **Type** | **Required** | **Restrictions** | **Description** |
| --- | --- | --- | --- | --- |
| username | string | true | none | Username belonging to account |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #6BBD5B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint does not require authentication</span> 
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.forgot_password import ForgotPassword
from clicksend.models.forgot_password_request import ForgotPasswordRequest
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
    api_instance = clicksend.VerificationOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    forgot_password_request = clicksend.ForgotPasswordRequest() # ForgotPasswordRequest |  (optional)

    try:
        # Forgot Password
        api_response = api_instance.forgot_password(content_type=content_type, forgot_password_request=forgot_password_request)
        print("The response of VerificationOtherApi->forgot_password:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VerificationOtherApi->forgot_password: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **forgot_password_request** | [**ForgotPasswordRequest**](ForgotPasswordRequest.md)|  | [optional] 

### Return type

[**ForgotPassword**](ForgotPassword.md)

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

# **forgot_username**
> ForgotUsername forgot_username(content_type=content_type, forgot_username_request=forgot_username_request)

Forgot Username

_Forgot username_

Requires the user to pass either the email registered to an account or the phone number, **not** both

### Properties

| **Name** | **Type** | **Required** | **Restrictions** | **Description** |
| --- | --- | --- | --- | --- |
| email | string | true | none | Email belonging to account |
| phone_number | string | true | none | Phone belonging to account |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #6BBD5B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint does not require authentication</span> 
</div>   

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.forgot_username import ForgotUsername
from clicksend.models.forgot_username_request import ForgotUsernameRequest
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
    api_instance = clicksend.VerificationOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    forgot_username_request = clicksend.ForgotUsernameRequest() # ForgotUsernameRequest |  (optional)

    try:
        # Forgot Username
        api_response = api_instance.forgot_username(content_type=content_type, forgot_username_request=forgot_username_request)
        print("The response of VerificationOtherApi->forgot_username:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VerificationOtherApi->forgot_username: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **forgot_username_request** | [**ForgotUsernameRequest**](ForgotUsernameRequest.md)|  | [optional] 

### Return type

[**ForgotUsername**](ForgotUsername.md)

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

