# clicksend.VoiceApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_voice_delivery_receipt_rule**](VoiceApi.md#create_voice_delivery_receipt_rule) | **POST** /v3/automations/voice/receipts | Create Voice Delivery Receipt Rule
[**delete_voice_delivery_receipt_rule**](VoiceApi.md#delete_voice_delivery_receipt_rule) | **DELETE** /v3/automations/voice/receipts/{receipt_rule_id} | Delete Voice Delivery Receipt Rule
[**update_voice_delivery_receipt_rule**](VoiceApi.md#update_voice_delivery_receipt_rule) | **PUT** /v3/automations/voice/receipts/{receipt_rule_id} | Update Voice Delivery Receipt Rule
[**view_voice_delivery_receipt_rule**](VoiceApi.md#view_voice_delivery_receipt_rule) | **GET** /v3/automations/voice/receipts/{receipt_rule_id} | View Voice Delivery Receipt Rule
[**view_voice_delivery_receipt_rules**](VoiceApi.md#view_voice_delivery_receipt_rules) | **GET** /v3/automations/voice/receipts | View Voice Delivery Receipt Rules


# **create_voice_delivery_receipt_rule**
> CreateVoiceDeliveryReceiptRule create_voice_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Create Voice Delivery Receipt Rule

_Create voice delivery receipt automations_

Create voice delivery receipt automations

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.models.create_voice_delivery_receipt_rule import CreateVoiceDeliveryReceiptRule
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
    api_instance = clicksend.VoiceApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Create Voice Delivery Receipt Rule
        api_response = api_instance.create_voice_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of VoiceApi->create_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceApi->create_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**CreateVoiceDeliveryReceiptRule**](CreateVoiceDeliveryReceiptRule.md)

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

# **delete_voice_delivery_receipt_rule**
> DeleteVoiceDeliveryReceiptRule delete_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

Delete Voice Delivery Receipt Rule

_Delete voice delivery receipt automation_

Delete voice delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_voice_delivery_receipt_rule import DeleteVoiceDeliveryReceiptRule
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
    api_instance = clicksend.VoiceApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Voice Delivery Receipt Rule
        api_response = api_instance.delete_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of VoiceApi->delete_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceApi->delete_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteVoiceDeliveryReceiptRule**](DeleteVoiceDeliveryReceiptRule.md)

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

# **update_voice_delivery_receipt_rule**
> UpdateVoiceDeliveryReceiptRule update_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Update Voice Delivery Receipt Rule

_Update voice delivery receipt automation_

Update voice delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.models.update_voice_delivery_receipt_rule import UpdateVoiceDeliveryReceiptRule
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
    api_instance = clicksend.VoiceApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Update Voice Delivery Receipt Rule
        api_response = api_instance.update_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of VoiceApi->update_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceApi->update_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**UpdateVoiceDeliveryReceiptRule**](UpdateVoiceDeliveryReceiptRule.md)

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

# **view_voice_delivery_receipt_rule**
> ViewVoiceDeliveryReceiptRule view_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

View Voice Delivery Receipt Rule

_Get specific voice delivery receipt automation_

Get specific voice delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_delivery_receipt_rule import ViewVoiceDeliveryReceiptRule
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
    api_instance = clicksend.VoiceApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Delivery Receipt Rule
        api_response = api_instance.view_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of VoiceApi->view_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceApi->view_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceDeliveryReceiptRule**](ViewVoiceDeliveryReceiptRule.md)

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

# **view_voice_delivery_receipt_rules**
> ViewVoiceDeliveryReceiptRules view_voice_delivery_receipt_rules(content_type=content_type)

View Voice Delivery Receipt Rules

_Get all voice delivery receipt automations_

Get all voice delivery receipt automations

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
from clicksend.models.view_voice_delivery_receipt_rules import ViewVoiceDeliveryReceiptRules
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
    api_instance = clicksend.VoiceApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Delivery Receipt Rules
        api_response = api_instance.view_voice_delivery_receipt_rules(content_type=content_type)
        print("The response of VoiceApi->view_voice_delivery_receipt_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VoiceApi->view_voice_delivery_receipt_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceDeliveryReceiptRules**](ViewVoiceDeliveryReceiptRules.md)

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

