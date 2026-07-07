# clicksend.EmailToSmsApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_allowed_email**](EmailToSmsApi.md#add_allowed_email) | **POST** /v3/sms/email-sms | Add Allowed Email
[**create_stripped_string_rule**](EmailToSmsApi.md#create_stripped_string_rule) | **POST** /v3/sms/email-sms-stripped-strings | Create Stripped String Rule
[**delete_stripped_string_rule**](EmailToSmsApi.md#delete_stripped_string_rule) | **DELETE** /v3/sms/email-sms-stripped-strings/{rule_id} | Delete Stripped String Rule
[**update_stripped_string_rule**](EmailToSmsApi.md#update_stripped_string_rule) | **PUT** /v3/sms/email-sms-stripped-strings/{rule_id} | Update Stripped String Rule
[**view_allowed_emails**](EmailToSmsApi.md#view_allowed_emails) | **GET** /v3/sms/email-sms | View Allowed Emails
[**view_stripped_string_rule**](EmailToSmsApi.md#view_stripped_string_rule) | **GET** /v3/sms/email-sms-stripped-strings/{rule_id} | View Stripped String Rule
[**view_stripped_string_rules**](EmailToSmsApi.md#view_stripped_string_rules) | **GET** /v3/sms/email-sms-stripped-strings | View Stripped String Rules


# **add_allowed_email**
> AddAllowedEmail add_allowed_email(content_type=content_type, add_allowed_email_request=add_allowed_email_request)

Add Allowed Email

_Create email to sms allowed address_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| email_address | string | true | none | Your email address |
| from | string | false | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.add_allowed_email import AddAllowedEmail
from clicksend.models.add_allowed_email_request import AddAllowedEmailRequest
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
    api_instance = clicksend.EmailToSmsApi(api_client)
    content_type = 'application/json' # str |  (optional)
    add_allowed_email_request = clicksend.AddAllowedEmailRequest() # AddAllowedEmailRequest |  (optional)

    try:
        # Add Allowed Email
        api_response = api_instance.add_allowed_email(content_type=content_type, add_allowed_email_request=add_allowed_email_request)
        print("The response of EmailToSmsApi->add_allowed_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailToSmsApi->add_allowed_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **add_allowed_email_request** | [**AddAllowedEmailRequest**](AddAllowedEmailRequest.md)|  | [optional] 

### Return type

[**AddAllowedEmail**](AddAllowedEmail.md)

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

# **create_stripped_string_rule**
> CreateStrippedStringRule create_stripped_string_rule(content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)

Create Stripped String Rule

_Create email to sms stripped string rule_

Create email to sms stripped string rules

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| stripped-string | body | string | true | String to be stripped. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_stripped_string_rule import CreateStrippedStringRule
from clicksend.models.create_stripped_string_rule_request import CreateStrippedStringRuleRequest
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
    api_instance = clicksend.EmailToSmsApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_stripped_string_rule_request = clicksend.CreateStrippedStringRuleRequest() # CreateStrippedStringRuleRequest |  (optional)

    try:
        # Create Stripped String Rule
        api_response = api_instance.create_stripped_string_rule(content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)
        print("The response of EmailToSmsApi->create_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailToSmsApi->create_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_stripped_string_rule_request** | [**CreateStrippedStringRuleRequest**](CreateStrippedStringRuleRequest.md)|  | [optional] 

### Return type

[**CreateStrippedStringRule**](CreateStrippedStringRule.md)

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

# **delete_stripped_string_rule**
> DeleteStrippedStringRule delete_stripped_string_rule(rule_id, content_type=content_type)

Delete Stripped String Rule

_Delete email to sms stripped string rule_

Delete email to sms stripped string rule

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| rule_id | path | integer(int32) | true | Your rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_stripped_string_rule import DeleteStrippedStringRule
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
    api_instance = clicksend.EmailToSmsApi(api_client)
    rule_id = 'rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Stripped String Rule
        api_response = api_instance.delete_stripped_string_rule(rule_id, content_type=content_type)
        print("The response of EmailToSmsApi->delete_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailToSmsApi->delete_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteStrippedStringRule**](DeleteStrippedStringRule.md)

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

# **update_stripped_string_rule**
> UpdateStrippedStringRule update_stripped_string_rule(rule_id, content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)

Update Stripped String Rule

_Update email to sms stripped string rule_

Update email to sms stripped string rule

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| rule_id | path | integer(int32) | true | Your rule id |
| stripped-string | body | string | true | String to be stripped. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_stripped_string_rule_request import CreateStrippedStringRuleRequest
from clicksend.models.update_stripped_string_rule import UpdateStrippedStringRule
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
    api_instance = clicksend.EmailToSmsApi(api_client)
    rule_id = 'rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_stripped_string_rule_request = clicksend.CreateStrippedStringRuleRequest() # CreateStrippedStringRuleRequest |  (optional)

    try:
        # Update Stripped String Rule
        api_response = api_instance.update_stripped_string_rule(rule_id, content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)
        print("The response of EmailToSmsApi->update_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailToSmsApi->update_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_stripped_string_rule_request** | [**CreateStrippedStringRuleRequest**](CreateStrippedStringRuleRequest.md)|  | [optional] 

### Return type

[**UpdateStrippedStringRule**](UpdateStrippedStringRule.md)

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

# **view_allowed_emails**
> ViewAllowedEmails view_allowed_emails(content_type=content_type)

View Allowed Emails

_Get list of email to sms allowed addresses_

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
from clicksend.models.view_allowed_emails import ViewAllowedEmails
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
    api_instance = clicksend.EmailToSmsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Allowed Emails
        api_response = api_instance.view_allowed_emails(content_type=content_type)
        print("The response of EmailToSmsApi->view_allowed_emails:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailToSmsApi->view_allowed_emails: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllowedEmails**](ViewAllowedEmails.md)

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

# **view_stripped_string_rule**
> ViewStrippedStringRule view_stripped_string_rule(rule_id, content_type=content_type)

View Stripped String Rule

_Get email to sms stripped string rule_

Get email to sms stripped string rule

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| rule_id | path | integer(int32) | true | Your rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_stripped_string_rule import ViewStrippedStringRule
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
    api_instance = clicksend.EmailToSmsApi(api_client)
    rule_id = 'rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Stripped String Rule
        api_response = api_instance.view_stripped_string_rule(rule_id, content_type=content_type)
        print("The response of EmailToSmsApi->view_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailToSmsApi->view_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewStrippedStringRule**](ViewStrippedStringRule.md)

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

# **view_stripped_string_rules**
> ViewStrippedStringRules view_stripped_string_rules(content_type=content_type)

View Stripped String Rules

_Get list of email to sms stripped string rules_

Get list of email to sms stripped string rules

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_stripped_string_rules import ViewStrippedStringRules
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
    api_instance = clicksend.EmailToSmsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Stripped String Rules
        api_response = api_instance.view_stripped_string_rules(content_type=content_type)
        print("The response of EmailToSmsApi->view_stripped_string_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailToSmsApi->view_stripped_string_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewStrippedStringRules**](ViewStrippedStringRules.md)

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

