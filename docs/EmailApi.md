# clicksend.EmailApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_email_campaign_price**](EmailApi.md#calculate_email_campaign_price) | **POST** /v3/email-campaigns/price | Calculate Email Campaign Price
[**calculate_email_price**](EmailApi.md#calculate_email_price) | **POST** /v3/email/price | Calculate Email Price
[**cancel_email_campaign**](EmailApi.md#cancel_email_campaign) | **PUT** /v3/email-campaigns/{email_campaign_id}/cancel | Cancel Email Campaign
[**create_allowed_email_address**](EmailApi.md#create_allowed_email_address) | **POST** /v3/email/addresses | Create Allowed Email Address
[**create_email_delivery_receipt_rule**](EmailApi.md#create_email_delivery_receipt_rule) | **POST** /v3/automations/email/receipts | Create Email Delivery Receipt Rule
[**create_email_template**](EmailApi.md#create_email_template) | **POST** /v3/email/templates | Create Email Template
[**delete_allowed_email_address**](EmailApi.md#delete_allowed_email_address) | **DELETE** /v3/email/addresses/{email_address_id} | Delete Allowed Email Address
[**delete_email_delivery_receipt_rule**](EmailApi.md#delete_email_delivery_receipt_rule) | **DELETE** /v3/automations/email/receipts/{receipt_rule_id} | Delete Email Delivery Receipt Rule
[**delete_email_template**](EmailApi.md#delete_email_template) | **DELETE** /v3/email/templates/{template_id} | Delete Email Template
[**export_email_campaign_history**](EmailApi.md#export_email_campaign_history) | **GET** /v3/email-campaigns/{email_campaign_id}/history/export | Export Email Campaign History
[**export_email_history**](EmailApi.md#export_email_history) | **GET** /v3/email/history/export | Export Email History
[**send_email**](EmailApi.md#send_email) | **POST** /v3/email/send | Send Email
[**send_email_campaign**](EmailApi.md#send_email_campaign) | **POST** /v3/email-campaigns/send | Send Email Campaign
[**send_email_verification_token**](EmailApi.md#send_email_verification_token) | **PUT** /v3/email/address-verify/{email_address_id}/send | Send Email Verification Token
[**update_email_campaign**](EmailApi.md#update_email_campaign) | **PUT** /v3/email-campaigns/{email_campaign_id} | Update Email Campaign
[**update_email_delivery_receipt_rule**](EmailApi.md#update_email_delivery_receipt_rule) | **PUT** /v3/automations/email/receipts/{receipt_rule_id} | Update Email Delivery Receipt Rule
[**update_email_template**](EmailApi.md#update_email_template) | **PUT** /v3/email/templates/{template_id} | Update Email Template
[**verify_allowed_email_address**](EmailApi.md#verify_allowed_email_address) | **PUT** /v3/email/address-verify/{email_address_id}/verify/{activation_token} | Verify Allowed Email Address
[**view_all_email_campaigns**](EmailApi.md#view_all_email_campaigns) | **GET** /v3/email-campaigns | View All Email Campaigns
[**view_allowed_email_address**](EmailApi.md#view_allowed_email_address) | **GET** /v3/email/addresses/{email_address_id} | View Allowed Email Address
[**view_allowed_email_addresses**](EmailApi.md#view_allowed_email_addresses) | **GET** /v3/email/addresses | View Allowed Email Addresses
[**view_email_campaign**](EmailApi.md#view_email_campaign) | **GET** /v3/email-campaigns/{email_campaign_id} | View Email Campaign
[**view_email_campaign_history**](EmailApi.md#view_email_campaign_history) | **GET** /v3/email-campaigns/{email_campaign_id}/history | View Email Campaign History
[**view_email_delivery_receipt_rule**](EmailApi.md#view_email_delivery_receipt_rule) | **GET** /v3/automations/email/receipts/{receipt_rule_id} | View Email Delivery Receipt Rule
[**view_email_delivery_receipt_rules**](EmailApi.md#view_email_delivery_receipt_rules) | **GET** /v3/automations/email/receipts | View Email Delivery Receipt Rules
[**view_email_history**](EmailApi.md#view_email_history) | **GET** /v3/email/history | View Email History
[**view_email_template**](EmailApi.md#view_email_template) | **GET** /v3/email/templates/{template_id} | View Email Template
[**view_email_templates**](EmailApi.md#view_email_templates) | **GET** /v3/email/templates | View Email Templates
[**view_master_email_template**](EmailApi.md#view_master_email_template) | **GET** /v3/email/master-templates/{template_id} | View Master Email Template
[**view_master_email_templates**](EmailApi.md#view_master_email_templates) | **GET** /v3/email/master-templates | View Master Email Templates
[**view_template_categories**](EmailApi.md#view_template_categories) | **GET** /v3/email/master-templates-categories | View Template Categories
[**view_template_category**](EmailApi.md#view_template_category) | **GET** /v3/email/master-templates-categories/{category_id} | View Template Category
[**view_templates_in_category**](EmailApi.md#view_templates_in_category) | **GET** /v3/email/master-templates-categories/{category_id}/master-templates | View Templates in Category


# **calculate_email_campaign_price**
> CalculateEmailCampaignPrice calculate_email_campaign_price(content_type=content_type, calculate_email_campaign_price_request=calculate_email_campaign_price_request)

Calculate Email Campaign Price

_Calculate email campaign price_

Calculate email campaign price

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| name | string | true | none | Your campaign name. |
| subject | string | true | none | Your campaign subject. |
| body | string | true | none | Your campaign message. |
| from_email_address_id | number | true | none | The allowed email address id. |
| from_name | string | true | none | Your name or business name. |
| template_id | number | false | none | Your template id. |
| list_id | number | true | none | Your contact list id. |
| schedule | integer(int32) | false | none | Your schedule timestamp. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_email_campaign_price import CalculateEmailCampaignPrice
from clicksend.models.calculate_email_campaign_price_request import CalculateEmailCampaignPriceRequest
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_email_campaign_price_request = clicksend.CalculateEmailCampaignPriceRequest() # CalculateEmailCampaignPriceRequest |  (optional)

    try:
        # Calculate Email Campaign Price
        api_response = api_instance.calculate_email_campaign_price(content_type=content_type, calculate_email_campaign_price_request=calculate_email_campaign_price_request)
        print("The response of EmailApi->calculate_email_campaign_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->calculate_email_campaign_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_email_campaign_price_request** | [**CalculateEmailCampaignPriceRequest**](CalculateEmailCampaignPriceRequest.md)|  | [optional] 

### Return type

[**CalculateEmailCampaignPrice**](CalculateEmailCampaignPrice.md)

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

# **calculate_email_price**
> CalculateEmailPrice calculate_email_price(content_type=content_type, calculate_email_price_request=calculate_email_price_request)

Calculate Email Price

_Get transactional email price_

Get transactional email price

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | array | true | none | Array of To Recipient items. (array of names and emails) |
| cc | array | false | none | Array of Cc Recipient items. (array of names and emails) |
| bcc | array | false | none | Array of Bcc Recipient items. (array of names and emails) |
| from | object | true | none | From Email object. (object containing name and email) |
| body | string | true | none | Body of the email. |
| attachments | array | false | none | Array of Attachment items. |
| schedule | number | false | none | Schedule. |
| name | string | false | none | Name of person email belongs to |
| email | string | true | none | Email to be used. |
| content | string | true | none | The base64-encoded contents of the file. |
| type | string | true | none | The type of file being attached. |
| filename | string | true | none | The name of the file being attached. |
| disposition | string | true | none | Inline for content that can be displayed within the email, or attachment for any other files. |
| content_id | string | true | none | An ID for the content. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_email_price import CalculateEmailPrice
from clicksend.models.calculate_email_price_request import CalculateEmailPriceRequest
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_email_price_request = clicksend.CalculateEmailPriceRequest() # CalculateEmailPriceRequest |  (optional)

    try:
        # Calculate Email Price
        api_response = api_instance.calculate_email_price(content_type=content_type, calculate_email_price_request=calculate_email_price_request)
        print("The response of EmailApi->calculate_email_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->calculate_email_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_email_price_request** | [**CalculateEmailPriceRequest**](CalculateEmailPriceRequest.md)|  | [optional] 

### Return type

[**CalculateEmailPrice**](CalculateEmailPrice.md)

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

# **cancel_email_campaign**
> CancelEmailCampaign cancel_email_campaign(email_campaign_id, content_type=content_type, cancel_email_campaign_request=cancel_email_campaign_request)

Cancel Email Campaign

_Cancel email campaign_

Cancel email campaign

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_campaign_id | path | integer(int32) | true | Allowed email campaign id |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
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
from clicksend.models.cancel_email_campaign import CancelEmailCampaign
from clicksend.models.cancel_email_campaign_request import CancelEmailCampaignRequest
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
    api_instance = clicksend.EmailApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    cancel_email_campaign_request = clicksend.CancelEmailCampaignRequest() # CancelEmailCampaignRequest |  (optional)

    try:
        # Cancel Email Campaign
        api_response = api_instance.cancel_email_campaign(email_campaign_id, content_type=content_type, cancel_email_campaign_request=cancel_email_campaign_request)
        print("The response of EmailApi->cancel_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->cancel_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **cancel_email_campaign_request** | [**CancelEmailCampaignRequest**](CancelEmailCampaignRequest.md)|  | [optional] 

### Return type

[**CancelEmailCampaign**](CancelEmailCampaign.md)

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

# **create_allowed_email_address**
> CreateAllowedEmailAddress create_allowed_email_address(content_type=content_type, create_allowed_email_address_request=create_allowed_email_address_request)

Create Allowed Email Address

_Create allowed Email Address_

Create allowed Email Address

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| body | body | string | true | Email to be allowed. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_allowed_email_address import CreateAllowedEmailAddress
from clicksend.models.create_allowed_email_address_request import CreateAllowedEmailAddressRequest
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_allowed_email_address_request = clicksend.CreateAllowedEmailAddressRequest() # CreateAllowedEmailAddressRequest |  (optional)

    try:
        # Create Allowed Email Address
        api_response = api_instance.create_allowed_email_address(content_type=content_type, create_allowed_email_address_request=create_allowed_email_address_request)
        print("The response of EmailApi->create_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->create_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_allowed_email_address_request** | [**CreateAllowedEmailAddressRequest**](CreateAllowedEmailAddressRequest.md)|  | [optional] 

### Return type

[**CreateAllowedEmailAddress**](CreateAllowedEmailAddress.md)

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

# **create_email_delivery_receipt_rule**
> CreateEmailDeliveryReceiptRule create_email_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Create Email Delivery Receipt Rule

_Create email delivery receipt automations_

Create email delivery receipt automations

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
from clicksend.models.create_email_delivery_receipt_rule import CreateEmailDeliveryReceiptRule
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Create Email Delivery Receipt Rule
        api_response = api_instance.create_email_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of EmailApi->create_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->create_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**CreateEmailDeliveryReceiptRule**](CreateEmailDeliveryReceiptRule.md)

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

# **create_email_template**
> CreateEmailTemplate create_email_template(content_type=content_type, create_email_template_request=create_email_template_request)

Create Email Template

_Create email template_

Create email template

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| template_name | string | true | none | The intended name for the new template. |
| template_id_master | number | true | none | The ID of the master template you want to base on. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_email_template import CreateEmailTemplate
from clicksend.models.create_email_template_request import CreateEmailTemplateRequest
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_email_template_request = clicksend.CreateEmailTemplateRequest() # CreateEmailTemplateRequest |  (optional)

    try:
        # Create Email Template
        api_response = api_instance.create_email_template(content_type=content_type, create_email_template_request=create_email_template_request)
        print("The response of EmailApi->create_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->create_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_email_template_request** | [**CreateEmailTemplateRequest**](CreateEmailTemplateRequest.md)|  | [optional] 

### Return type

[**CreateEmailTemplate**](CreateEmailTemplate.md)

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

# **delete_allowed_email_address**
> DeleteAllowedEmailAddress delete_allowed_email_address(email_address_id, content_type=content_type)

Delete Allowed Email Address

_Delete specific email address_

Delete specific email address

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_allowed_email_address import DeleteAllowedEmailAddress
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
    api_instance = clicksend.EmailApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Allowed Email Address
        api_response = api_instance.delete_allowed_email_address(email_address_id, content_type=content_type)
        print("The response of EmailApi->delete_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->delete_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteAllowedEmailAddress**](DeleteAllowedEmailAddress.md)

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

# **delete_email_delivery_receipt_rule**
> DeleteEmailDeliveryReceiptRule delete_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

Delete Email Delivery Receipt Rule

_Delete email delivery receipt automation_

Delete email delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_email_delivery_receipt_rule import DeleteEmailDeliveryReceiptRule
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
    api_instance = clicksend.EmailApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Email Delivery Receipt Rule
        api_response = api_instance.delete_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of EmailApi->delete_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->delete_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteEmailDeliveryReceiptRule**](DeleteEmailDeliveryReceiptRule.md)

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

# **delete_email_template**
> DeleteEmailTemplate delete_email_template(template_id, content_type=content_type)

Delete Email Template

_Delete user email template_

Delete user email template

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_email_template import DeleteEmailTemplate
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
    api_instance = clicksend.EmailApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Email Template
        api_response = api_instance.delete_email_template(template_id, content_type=content_type)
        print("The response of EmailApi->delete_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->delete_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteEmailTemplate**](DeleteEmailTemplate.md)

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

# **export_email_campaign_history**
> export_email_campaign_history(email_campaign_id, content_type=content_type)

Export Email Campaign History

_Export specific email campaign history_

Export specific email campaign history

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_campaign_id | path | integer(int32) | true | Allowed email campaign id |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
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
    api_instance = clicksend.EmailApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Export Email Campaign History
        api_instance.export_email_campaign_history(email_campaign_id, content_type=content_type)
    except Exception as e:
        print("Exception when calling EmailApi->export_email_campaign_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

void (empty response body)

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

# **export_email_history**
> ExportEmailHistory export_email_history(content_type=content_type)

Export Email History

_Export all Transactional Email history_

Export all Transactional Email history

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to download history as |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_email_history import ExportEmailHistory
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Export Email History
        api_response = api_instance.export_email_history(content_type=content_type)
        print("The response of EmailApi->export_email_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->export_email_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ExportEmailHistory**](ExportEmailHistory.md)

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

# **send_email**
> SendEmail send_email(content_type=content_type, send_email_request=send_email_request)

Send Email

_Send transactional email_

Send transactional email

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | array | true | none | Array of To Recipient items. (array of names and emails) |
| cc | array | false | none | Array of Cc Recipient items. (array of names and emails) |
| bcc | array | false | none | Array of Bcc Recipient items. (array of names and emails) |
| from | object | true | none | From Email object. (object containing name and email) |
| body | string | true | none | Body of the email. |
| attachments | array | false | none | Array of Attachment items. |
| schedule | number | false | none | Schedule. |
| name | string | false | none | Name of person email belongs to |
| email | string | true | none | Email to be used. |
| content | string | true | none | The base64-encoded contents of the file. |
| type | string | true | none | The type of file being attached. |
| filename | string | true | none | The name of the file being attached. |
| disposition | string | true | none | Inline for content that can be displayed within the email, or attachment for any other files. |
| content_id | string | true | none | An ID for the content. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_email import SendEmail
from clicksend.models.send_email_request import SendEmailRequest
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_email_request = clicksend.SendEmailRequest() # SendEmailRequest |  (optional)

    try:
        # Send Email
        api_response = api_instance.send_email(content_type=content_type, send_email_request=send_email_request)
        print("The response of EmailApi->send_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->send_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_email_request** | [**SendEmailRequest**](SendEmailRequest.md)|  | [optional] 

### Return type

[**SendEmail**](SendEmail.md)

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

# **send_email_campaign**
> SendEmailCampaign send_email_campaign(content_type=content_type, send_email_campaign_request=send_email_campaign_request)

Send Email Campaign

_Send email campaign_

Send email campaign

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| name | string | true | none | Your campaign name. |
| subject | string | true | none | Your campaign subject. |
| body | string | true | none | Your campaign message. |
| from_email_address_id | number | true | none | The allowed email address id. |
| from_name | string | true | none | Your name or business name. |
| template_id | number | false | none | Your template id. |
| list_id | number | true | none | Your contact list id. |
| schedule | integer(int32) | false | none | Your schedule timestamp. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_email_campaign import SendEmailCampaign
from clicksend.models.send_email_campaign_request import SendEmailCampaignRequest
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_email_campaign_request = clicksend.SendEmailCampaignRequest() # SendEmailCampaignRequest |  (optional)

    try:
        # Send Email Campaign
        api_response = api_instance.send_email_campaign(content_type=content_type, send_email_campaign_request=send_email_campaign_request)
        print("The response of EmailApi->send_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->send_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_email_campaign_request** | [**SendEmailCampaignRequest**](SendEmailCampaignRequest.md)|  | [optional] 

### Return type

[**SendEmailCampaign**](SendEmailCampaign.md)

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

# **send_email_verification_token**
> SendEmailVerificationToken send_email_verification_token(email_address_id, content_type=content_type, send_email_verification_token_request=send_email_verification_token_request)

Send Email Verification Token

_Send verification token_

Send verification token

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_email_verification_token import SendEmailVerificationToken
from clicksend.models.send_email_verification_token_request import SendEmailVerificationTokenRequest
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
    api_instance = clicksend.EmailApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    send_email_verification_token_request = clicksend.SendEmailVerificationTokenRequest() # SendEmailVerificationTokenRequest |  (optional)

    try:
        # Send Email Verification Token
        api_response = api_instance.send_email_verification_token(email_address_id, content_type=content_type, send_email_verification_token_request=send_email_verification_token_request)
        print("The response of EmailApi->send_email_verification_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->send_email_verification_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **send_email_verification_token_request** | [**SendEmailVerificationTokenRequest**](SendEmailVerificationTokenRequest.md)|  | [optional] 

### Return type

[**SendEmailVerificationToken**](SendEmailVerificationToken.md)

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

# **update_email_campaign**
> UpdateEmailCampaign update_email_campaign(email_campaign_id, content_type=content_type, update_email_campaign_request=update_email_campaign_request)

Update Email Campaign

_Edit email campaign_

Edit email campaign

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_campaign_id | path | integer(int32) | true | Allowed email campaign id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_email_campaign import UpdateEmailCampaign
from clicksend.models.update_email_campaign_request import UpdateEmailCampaignRequest
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
    api_instance = clicksend.EmailApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_email_campaign_request = clicksend.UpdateEmailCampaignRequest() # UpdateEmailCampaignRequest |  (optional)

    try:
        # Update Email Campaign
        api_response = api_instance.update_email_campaign(email_campaign_id, content_type=content_type, update_email_campaign_request=update_email_campaign_request)
        print("The response of EmailApi->update_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->update_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_email_campaign_request** | [**UpdateEmailCampaignRequest**](UpdateEmailCampaignRequest.md)|  | [optional] 

### Return type

[**UpdateEmailCampaign**](UpdateEmailCampaign.md)

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

# **update_email_delivery_receipt_rule**
> UpdateEmailDeliveryReceiptRule update_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Update Email Delivery Receipt Rule

_Update email delivery receipt automation_

Update email delivery receipt automation

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
from clicksend.models.update_email_delivery_receipt_rule import UpdateEmailDeliveryReceiptRule
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
    api_instance = clicksend.EmailApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Update Email Delivery Receipt Rule
        api_response = api_instance.update_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of EmailApi->update_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->update_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**UpdateEmailDeliveryReceiptRule**](UpdateEmailDeliveryReceiptRule.md)

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

# **update_email_template**
> UpdateEmailTemplate update_email_template(template_id, content_type=content_type, update_email_template_request=update_email_template_request)

Update Email Template

_Update email template_

Update email template

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| template_name | string | false | none | The intended name for the template. |
| body | string | true | none | Your template body. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_email_template import UpdateEmailTemplate
from clicksend.models.update_email_template_request import UpdateEmailTemplateRequest
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
    api_instance = clicksend.EmailApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_email_template_request = clicksend.UpdateEmailTemplateRequest() # UpdateEmailTemplateRequest |  (optional)

    try:
        # Update Email Template
        api_response = api_instance.update_email_template(template_id, content_type=content_type, update_email_template_request=update_email_template_request)
        print("The response of EmailApi->update_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->update_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_email_template_request** | [**UpdateEmailTemplateRequest**](UpdateEmailTemplateRequest.md)|  | [optional] 

### Return type

[**UpdateEmailTemplate**](UpdateEmailTemplate.md)

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

# **verify_allowed_email_address**
> VerifyAllowedEmailAddress verify_allowed_email_address(email_address_id, activation_token, content_type=content_type, verify_allowed_email_address_request=verify_allowed_email_address_request)

Verify Allowed Email Address

_Verify email address using verification token_

Verify email address using verification token

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |
| activation_token | path | string | true | Your activation token. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.verify_allowed_email_address import VerifyAllowedEmailAddress
from clicksend.models.verify_allowed_email_address_request import VerifyAllowedEmailAddressRequest
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
    api_instance = clicksend.EmailApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    activation_token = 'activation_token_example' # str | 
    content_type = 'application/json' # str |  (optional)
    verify_allowed_email_address_request = clicksend.VerifyAllowedEmailAddressRequest() # VerifyAllowedEmailAddressRequest |  (optional)

    try:
        # Verify Allowed Email Address
        api_response = api_instance.verify_allowed_email_address(email_address_id, activation_token, content_type=content_type, verify_allowed_email_address_request=verify_allowed_email_address_request)
        print("The response of EmailApi->verify_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->verify_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **activation_token** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **verify_allowed_email_address_request** | [**VerifyAllowedEmailAddressRequest**](VerifyAllowedEmailAddressRequest.md)|  | [optional] 

### Return type

[**VerifyAllowedEmailAddress**](VerifyAllowedEmailAddress.md)

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

# **view_all_email_campaigns**
> ViewAllEmailCampaigns view_all_email_campaigns(content_type=content_type)

View All Email Campaigns

_Get all email campaigns_

Get all email campaigns

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
from clicksend.models.view_all_email_campaigns import ViewAllEmailCampaigns
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View All Email Campaigns
        api_response = api_instance.view_all_email_campaigns(content_type=content_type)
        print("The response of EmailApi->view_all_email_campaigns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_all_email_campaigns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllEmailCampaigns**](ViewAllEmailCampaigns.md)

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

# **view_allowed_email_address**
> ViewAllowedEmailAddress view_allowed_email_address(email_address_id, content_type=content_type)

View Allowed Email Address

_Get specific email address_

Get specific email address

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_allowed_email_address import ViewAllowedEmailAddress
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
    api_instance = clicksend.EmailApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Allowed Email Address
        api_response = api_instance.view_allowed_email_address(email_address_id, content_type=content_type)
        print("The response of EmailApi->view_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllowedEmailAddress**](ViewAllowedEmailAddress.md)

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

# **view_allowed_email_addresses**
> ViewAllowedEmailAddresses view_allowed_email_addresses(content_type=content_type)

View Allowed Email Addresses

_Get all email addresses_

Get all email addresses

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
from clicksend.models.view_allowed_email_addresses import ViewAllowedEmailAddresses
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Allowed Email Addresses
        api_response = api_instance.view_allowed_email_addresses(content_type=content_type)
        print("The response of EmailApi->view_allowed_email_addresses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_allowed_email_addresses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllowedEmailAddresses**](ViewAllowedEmailAddresses.md)

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

# **view_email_campaign**
> ViewEmailCampaign view_email_campaign(email_campaign_id, content_type=content_type)

View Email Campaign

_Get specific email campaign_

Get specific email campaign

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_campaign import ViewEmailCampaign
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
    api_instance = clicksend.EmailApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Campaign
        api_response = api_instance.view_email_campaign(email_campaign_id, content_type=content_type)
        print("The response of EmailApi->view_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailCampaign**](ViewEmailCampaign.md)

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

# **view_email_campaign_history**
> ViewEmailCampaignHistory view_email_campaign_history(email_campaign_id, content_type=content_type)

View Email Campaign History

_Get specific email campaign history_

Get specific email campaign history


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_campaign_history import ViewEmailCampaignHistory
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
    api_instance = clicksend.EmailApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Campaign History
        api_response = api_instance.view_email_campaign_history(email_campaign_id, content_type=content_type)
        print("The response of EmailApi->view_email_campaign_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_email_campaign_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailCampaignHistory**](ViewEmailCampaignHistory.md)

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

# **view_email_delivery_receipt_rule**
> ViewEmailDeliveryReceiptRule view_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

View Email Delivery Receipt Rule

_Get specific email delivery receipt automation_

Get specific email delivery receipt automation

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
from clicksend.models.view_email_delivery_receipt_rule import ViewEmailDeliveryReceiptRule
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
    api_instance = clicksend.EmailApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Delivery Receipt Rule
        api_response = api_instance.view_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of EmailApi->view_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailDeliveryReceiptRule**](ViewEmailDeliveryReceiptRule.md)

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

# **view_email_delivery_receipt_rules**
> ViewEmailDeliveryReceiptRules view_email_delivery_receipt_rules(content_type=content_type)

View Email Delivery Receipt Rules

_Get all email delivery receipt automations_

Get all email delivery receipt automations

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
from clicksend.models.view_email_delivery_receipt_rules import ViewEmailDeliveryReceiptRules
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Delivery Receipt Rules
        api_response = api_instance.view_email_delivery_receipt_rules(content_type=content_type)
        print("The response of EmailApi->view_email_delivery_receipt_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_email_delivery_receipt_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailDeliveryReceiptRules**](ViewEmailDeliveryReceiptRules.md)

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

# **view_email_history**
> ViewEmailHistory view_email_history(content_type=content_type)

View Email History

_Get all transactional email history_

Get all transactional email history

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
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
from clicksend.models.view_email_history import ViewEmailHistory
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email History
        api_response = api_instance.view_email_history(content_type=content_type)
        print("The response of EmailApi->view_email_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_email_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailHistory**](ViewEmailHistory.md)

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

# **view_email_template**
> ViewEmailTemplate view_email_template(template_id, content_type=content_type)

View Email Template

_Get specific user email template_

Get specific user email templates

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_template import ViewEmailTemplate
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
    api_instance = clicksend.EmailApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Template
        api_response = api_instance.view_email_template(template_id, content_type=content_type)
        print("The response of EmailApi->view_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailTemplate**](ViewEmailTemplate.md)

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

# **view_email_templates**
> ViewEmailTemplates view_email_templates(content_type=content_type)

View Email Templates

_Get all user email templates_

Get all user email templates

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
from clicksend.models.view_email_templates import ViewEmailTemplates
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Templates
        api_response = api_instance.view_email_templates(content_type=content_type)
        print("The response of EmailApi->view_email_templates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_email_templates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailTemplates**](ViewEmailTemplates.md)

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

# **view_master_email_template**
> ViewMasterEmailTemplate view_master_email_template(template_id, content_type=content_type)

View Master Email Template

_Get specific master email template_

Get specific master email template

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_master_email_template import ViewMasterEmailTemplate
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
    api_instance = clicksend.EmailApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Master Email Template
        api_response = api_instance.view_master_email_template(template_id, content_type=content_type)
        print("The response of EmailApi->view_master_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_master_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewMasterEmailTemplate**](ViewMasterEmailTemplate.md)

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

# **view_master_email_templates**
> ViewMasterEmailTemplates view_master_email_templates(content_type=content_type)

View Master Email Templates

_Get all master email templates._

Get all master email templates.

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
from clicksend.models.view_master_email_templates import ViewMasterEmailTemplates
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Master Email Templates
        api_response = api_instance.view_master_email_templates(content_type=content_type)
        print("The response of EmailApi->view_master_email_templates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_master_email_templates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewMasterEmailTemplates**](ViewMasterEmailTemplates.md)

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

# **view_template_categories**
> ViewTemplateCategories view_template_categories(content_type=content_type)

View Template Categories

_Get all master email template categories_

Get all master email template categories

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
from clicksend.models.view_template_categories import ViewTemplateCategories
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
    api_instance = clicksend.EmailApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Template Categories
        api_response = api_instance.view_template_categories(content_type=content_type)
        print("The response of EmailApi->view_template_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_template_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewTemplateCategories**](ViewTemplateCategories.md)

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

# **view_template_category**
> ViewTemplateCategory view_template_category(category_id, content_type=content_type)

View Template Category

_Get specific master email template category_

Get specific master email template category

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| category_id | path | integer(int32) | true | Email category id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_template_category import ViewTemplateCategory
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
    api_instance = clicksend.EmailApi(api_client)
    category_id = 'category_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Template Category
        api_response = api_instance.view_template_category(category_id, content_type=content_type)
        print("The response of EmailApi->view_template_category:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_template_category: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewTemplateCategory**](ViewTemplateCategory.md)

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

# **view_templates_in_category**
> ViewTemplatesInCategory view_templates_in_category(category_id, content_type=content_type)

View Templates in Category

_Get all master email templates in a category_

Get all master email templates in a category

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| category_id | path | integer(int32) | true | Email category id |
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
from clicksend.models.view_templates_in_category import ViewTemplatesInCategory
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
    api_instance = clicksend.EmailApi(api_client)
    category_id = 'category_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Templates in Category
        api_response = api_instance.view_templates_in_category(category_id, content_type=content_type)
        print("The response of EmailApi->view_templates_in_category:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->view_templates_in_category: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewTemplatesInCategory**](ViewTemplatesInCategory.md)

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

