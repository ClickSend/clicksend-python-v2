# clicksend.FaxOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_fax_price**](FaxOtherApi.md#calculate_fax_price) | **POST** /v3/fax/price | Calculate Fax Price
[**create_fax_delivery_receipt_rule**](FaxOtherApi.md#create_fax_delivery_receipt_rule) | **POST** /v3/automations/fax/receipts | Create FAX Delivery Receipt Rule
[**create_fax_inbound_rule**](FaxOtherApi.md#create_fax_inbound_rule) | **POST** /v3/automations/fax/inbound | Create Fax Inbound Rule
[**delete_fax_delivery_receipt_rule**](FaxOtherApi.md#delete_fax_delivery_receipt_rule) | **DELETE** /v3/automations/fax/receipts/{receipt_rule_id} | Delete FAX Delivery Receipt Rule
[**delete_fax_inbound_rule**](FaxOtherApi.md#delete_fax_inbound_rule) | **DELETE** /v3/automations/fax/inbound/{inbound_rule_id} | Delete Fax Inbound Rule
[**send_fax**](FaxOtherApi.md#send_fax) | **POST** /v3/fax/send | Send Fax
[**update_fax_delivery_receipt_rule**](FaxOtherApi.md#update_fax_delivery_receipt_rule) | **PUT** /v3/automations/fax/receipts/{receipt_rule_id} | Update FAX Delivery Receipt Rule
[**update_fax_inbound_rule**](FaxOtherApi.md#update_fax_inbound_rule) | **PUT** /v3/automations/fax/inbound/{inbound_rule_id} | Update Fax Inbound Rule
[**view_fax_delivery_receipt_rule**](FaxOtherApi.md#view_fax_delivery_receipt_rule) | **GET** /v3/automations/fax/receipts/{receipt_rule_id} | View FAX Delivery Receipt Rule
[**view_fax_delivery_receipt_rules**](FaxOtherApi.md#view_fax_delivery_receipt_rules) | **GET** /v3/automations/fax/receipts | View FAX Delivery Receipt Rules
[**view_fax_history**](FaxOtherApi.md#view_fax_history) | **GET** /v3/fax/history | View Fax History
[**view_fax_inbound_rule**](FaxOtherApi.md#view_fax_inbound_rule) | **GET** /v3/automations/fax/inbound/{inbound_rule_id} | View Fax Inbound Rule
[**view_fax_inbound_rules**](FaxOtherApi.md#view_fax_inbound_rules) | **GET** /v3/automations/fax/inbound | View Fax Inbound Rules
[**view_fax_receipts**](FaxOtherApi.md#view_fax_receipts) | **GET** /v3/fax/receipts | View Fax Receipts
[**view_specific_fax_receipt**](FaxOtherApi.md#view_specific_fax_receipt) | **GET** /v3/fax/receipts/{message_id} | View Specific Fax Receipt


# **calculate_fax_price**
> CalculateFaxPrice calculate_fax_price(content_type=content_type, calculate_fax_price_request=calculate_fax_price_request)

Calculate Fax Price

_Calculate Total Price for Fax Messages sent_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| source | string | true | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| to | string | true | none | Recipient fax number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id. Must be a valid fax number. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| custom_string | string | false | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | false | none | ISO alpha-2 character country code e.g. 'US', we use this to format the recipient number if it's not in international format. |
| from_email | string | false | none | An email address where the reply should be emailed to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_fax_price import CalculateFaxPrice
from clicksend.models.calculate_fax_price_request import CalculateFaxPriceRequest
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_fax_price_request = clicksend.CalculateFaxPriceRequest() # CalculateFaxPriceRequest |  (optional)

    try:
        # Calculate Fax Price
        api_response = api_instance.calculate_fax_price(content_type=content_type, calculate_fax_price_request=calculate_fax_price_request)
        print("The response of FaxOtherApi->calculate_fax_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->calculate_fax_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_fax_price_request** | [**CalculateFaxPriceRequest**](CalculateFaxPriceRequest.md)|  | [optional] 

### Return type

[**CalculateFaxPrice**](CalculateFaxPrice.md)

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

# **create_fax_delivery_receipt_rule**
> CreateFaxDeliveryReceiptRule create_fax_delivery_receipt_rule(content_type=content_type, create_fax_delivery_receipt_rule_request=create_fax_delivery_receipt_rule_request)

Create FAX Delivery Receipt Rule

_Create fax delivery receipt automations_

Create fax delivery receipt automations

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
from clicksend.models.create_fax_delivery_receipt_rule import CreateFaxDeliveryReceiptRule
from clicksend.models.create_fax_delivery_receipt_rule_request import CreateFaxDeliveryReceiptRuleRequest
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_fax_delivery_receipt_rule_request = clicksend.CreateFaxDeliveryReceiptRuleRequest() # CreateFaxDeliveryReceiptRuleRequest |  (optional)

    try:
        # Create FAX Delivery Receipt Rule
        api_response = api_instance.create_fax_delivery_receipt_rule(content_type=content_type, create_fax_delivery_receipt_rule_request=create_fax_delivery_receipt_rule_request)
        print("The response of FaxOtherApi->create_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->create_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_fax_delivery_receipt_rule_request** | [**CreateFaxDeliveryReceiptRuleRequest**](CreateFaxDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**CreateFaxDeliveryReceiptRule**](CreateFaxDeliveryReceiptRule.md)

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

# **create_fax_inbound_rule**
> CreateFaxInboundRule create_fax_inbound_rule(content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)

Create Fax Inbound Rule

_Create new inbound fax automation_

Create new inbound fax automation

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | string | true | none | Dedicated Number. Can be '\*' to apply to all numbers. |
| rule_name | string | true | none | Rule Name. |
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
from clicksend.models.create_fax_inbound_rule import CreateFaxInboundRule
from clicksend.models.create_fax_inbound_rule_request import CreateFaxInboundRuleRequest
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_fax_inbound_rule_request = clicksend.CreateFaxInboundRuleRequest() # CreateFaxInboundRuleRequest |  (optional)

    try:
        # Create Fax Inbound Rule
        api_response = api_instance.create_fax_inbound_rule(content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)
        print("The response of FaxOtherApi->create_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->create_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_fax_inbound_rule_request** | [**CreateFaxInboundRuleRequest**](CreateFaxInboundRuleRequest.md)|  | [optional] 

### Return type

[**CreateFaxInboundRule**](CreateFaxInboundRule.md)

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

# **delete_fax_delivery_receipt_rule**
> DeleteFaxDeliveryReceiptRule delete_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

Delete FAX Delivery Receipt Rule

_Delete fax delivery receipt automation_

Delete fax delivery receipt automation

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
from clicksend.models.delete_fax_delivery_receipt_rule import DeleteFaxDeliveryReceiptRule
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
    api_instance = clicksend.FaxOtherApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete FAX Delivery Receipt Rule
        api_response = api_instance.delete_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of FaxOtherApi->delete_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->delete_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteFaxDeliveryReceiptRule**](DeleteFaxDeliveryReceiptRule.md)

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

# **delete_fax_inbound_rule**
> DeleteFaxInboundRule delete_fax_inbound_rule(inbound_rule_id, content_type=content_type)

Delete Fax Inbound Rule

_Delete inbound fax automation_

Delete inbound fax automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_fax_inbound_rule import DeleteFaxInboundRule
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
    api_instance = clicksend.FaxOtherApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Fax Inbound Rule
        api_response = api_instance.delete_fax_inbound_rule(inbound_rule_id, content_type=content_type)
        print("The response of FaxOtherApi->delete_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->delete_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteFaxInboundRule**](DeleteFaxInboundRule.md)

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

# **send_fax**
> SendFax send_fax(content_type=content_type, send_fax_request=send_fax_request)

Send Fax

### **Supported File Types**

- Supported file types are listed below. If you need to convert a file to a supported format, it can be first passed to our uploads endpoint: `/uploads?convert=fax`
- This will return a URL to the converted pdf file that can be used in the /fax/send endpoint.
- Contact us to add support for any other file type.
    

### Documents

| File type | Required to be passed to uploads endpoint first? |
| --- | --- |
| pdf | No |
| docx | Yes |
| doc | Yes |
| rtf | Yes |

_Send a fax using supplied supported file-types._

### **Letter File Options**

### Use existing URL

With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.

When using an existing url make sure that it is publicly accessible as it will not work if it is private.

### Upload File to Our Server

With this option, you can use the [/uploads](/#upload-media-file) endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| source | string | true | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| to | string | true | none | Recipient fax number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id. Must be a valid fax number. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| custom_string | string | false | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | false | none | ISO alpha-2 character country code e.g. 'US', we use this to format the recipient number if it's not in international format. |
| from_email | string | false | none | An email address where the reply should be emailed to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_fax import SendFax
from clicksend.models.send_fax_request import SendFaxRequest
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_fax_request = clicksend.SendFaxRequest() # SendFaxRequest |  (optional)

    try:
        # Send Fax
        api_response = api_instance.send_fax(content_type=content_type, send_fax_request=send_fax_request)
        print("The response of FaxOtherApi->send_fax:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->send_fax: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_fax_request** | [**SendFaxRequest**](SendFaxRequest.md)|  | [optional] 

### Return type

[**SendFax**](SendFax.md)

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

# **update_fax_delivery_receipt_rule**
> UpdateFaxDeliveryReceiptRule update_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type, update_fax_delivery_receipt_rule_request=update_fax_delivery_receipt_rule_request)

Update FAX Delivery Receipt Rule

_Update fax delivery receipt automation_

Update fax delivery receipt automation

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
from clicksend.models.update_fax_delivery_receipt_rule import UpdateFaxDeliveryReceiptRule
from clicksend.models.update_fax_delivery_receipt_rule_request import UpdateFaxDeliveryReceiptRuleRequest
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
    api_instance = clicksend.FaxOtherApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_fax_delivery_receipt_rule_request = clicksend.UpdateFaxDeliveryReceiptRuleRequest() # UpdateFaxDeliveryReceiptRuleRequest |  (optional)

    try:
        # Update FAX Delivery Receipt Rule
        api_response = api_instance.update_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type, update_fax_delivery_receipt_rule_request=update_fax_delivery_receipt_rule_request)
        print("The response of FaxOtherApi->update_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->update_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_fax_delivery_receipt_rule_request** | [**UpdateFaxDeliveryReceiptRuleRequest**](UpdateFaxDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**UpdateFaxDeliveryReceiptRule**](UpdateFaxDeliveryReceiptRule.md)

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

# **update_fax_inbound_rule**
> UpdateFaxInboundRule update_fax_inbound_rule(inbound_rule_id, content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)

Update Fax Inbound Rule

_Update inbound fax automation_

Update inbound fax automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | string | true | none | Dedicated Number. Can be '\*' to apply to all numbers. |
| rule_name | string | true | none | Rule Name. |
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
from clicksend.models.create_fax_inbound_rule_request import CreateFaxInboundRuleRequest
from clicksend.models.update_fax_inbound_rule import UpdateFaxInboundRule
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
    api_instance = clicksend.FaxOtherApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_fax_inbound_rule_request = clicksend.CreateFaxInboundRuleRequest() # CreateFaxInboundRuleRequest |  (optional)

    try:
        # Update Fax Inbound Rule
        api_response = api_instance.update_fax_inbound_rule(inbound_rule_id, content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)
        print("The response of FaxOtherApi->update_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->update_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_fax_inbound_rule_request** | [**CreateFaxInboundRuleRequest**](CreateFaxInboundRuleRequest.md)|  | [optional] 

### Return type

[**UpdateFaxInboundRule**](UpdateFaxInboundRule.md)

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

# **view_fax_delivery_receipt_rule**
> ViewFaxDeliveryReceiptRule view_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

View FAX Delivery Receipt Rule

_Get specific fax delivery receipt automation_

Get specific fax delivery receipt automation

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
from clicksend.models.view_fax_delivery_receipt_rule import ViewFaxDeliveryReceiptRule
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
    api_instance = clicksend.FaxOtherApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View FAX Delivery Receipt Rule
        api_response = api_instance.view_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of FaxOtherApi->view_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->view_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxDeliveryReceiptRule**](ViewFaxDeliveryReceiptRule.md)

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

# **view_fax_delivery_receipt_rules**
> ViewFaxDeliveryReceiptRules view_fax_delivery_receipt_rules(content_type=content_type)

View FAX Delivery Receipt Rules

_Get all fax delivery receipt automations_

Get all fax delivery receipt automations

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
from clicksend.models.view_fax_delivery_receipt_rules import ViewFaxDeliveryReceiptRules
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View FAX Delivery Receipt Rules
        api_response = api_instance.view_fax_delivery_receipt_rules(content_type=content_type)
        print("The response of FaxOtherApi->view_fax_delivery_receipt_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->view_fax_delivery_receipt_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxDeliveryReceiptRules**](ViewFaxDeliveryReceiptRules.md)

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

# **view_fax_history**
> ViewFaxHistory view_fax_history(content_type=content_type)

View Fax History

_Get a list of Fax History._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
| q | query | string | false | Custom query Example: status:Sent,status_code:201. |
| order | query | string | false | Order result by Example: date_added:desc,list_id:desc. |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |

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
from clicksend.models.view_fax_history import ViewFaxHistory
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax History
        api_response = api_instance.view_fax_history(content_type=content_type)
        print("The response of FaxOtherApi->view_fax_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->view_fax_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxHistory**](ViewFaxHistory.md)

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

# **view_fax_inbound_rule**
> ViewFaxInboundRule view_fax_inbound_rule(inbound_rule_id, content_type=content_type)

View Fax Inbound Rule

_Get specific inbound fax automation_

Get specific inbound fax automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_inbound_rule import ViewFaxInboundRule
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
    api_instance = clicksend.FaxOtherApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax Inbound Rule
        api_response = api_instance.view_fax_inbound_rule(inbound_rule_id, content_type=content_type)
        print("The response of FaxOtherApi->view_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->view_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxInboundRule**](ViewFaxInboundRule.md)

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

# **view_fax_inbound_rules**
> ViewFaxInboundRules view_fax_inbound_rules(content_type=content_type)

View Fax Inbound Rules

_Get all inbound fax automations_

Get all inbound fax automations

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
from clicksend.models.view_fax_inbound_rules import ViewFaxInboundRules
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax Inbound Rules
        api_response = api_instance.view_fax_inbound_rules(content_type=content_type)
        print("The response of FaxOtherApi->view_fax_inbound_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->view_fax_inbound_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxInboundRules**](ViewFaxInboundRules.md)

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

# **view_fax_receipts**
> ViewFaxReceipts view_fax_receipts(content_type=content_type)

View Fax Receipts

_Get List of Fax Receipts_

**Push Delivery Receipts**

If you prefer, we can push message replies to your server as they arrive with us.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Fax then Delivery Reports.
5. Click the 'Add New Rule' button.
6. Select the 'URL' action.
7. Enter the URL and click 'Save'.
    

The following variables will be posted to the URL specified:

| Variable | Description |
| --- | --- |
| `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980 |
| `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981 |
| `message_id` | Message ID, returned when originally sending the message. |
| `status` | Delivered or Undelivered |
| `status_code` | Status code. Refer to 'Fax Delivery Status Codes' in docs. |
| `status_text` | Status text. |
| `error_code` | Error code. |
| `error_text` | Error text. |
| `custom_string` | A custom string used when sending the original message. |
| `user_id` | The user ID of the user who sent the message. |
| `subaccount_id` | The subaccount ID of the user who sent the message. |
| `message_type` | 'fax' (constant). |

**Pull Delivery Receipts**

Receive delivery reports by polling. You can poll our server and retrieve delivery reports at a time that suits you.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Fax then Delivery Rules.
5. Click the 'Add New Rule' button.
6. Select the 'Poll' action.
7. Then click 'Save'.
    

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_receipts import ViewFaxReceipts
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
    api_instance = clicksend.FaxOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax Receipts
        api_response = api_instance.view_fax_receipts(content_type=content_type)
        print("The response of FaxOtherApi->view_fax_receipts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->view_fax_receipts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxReceipts**](ViewFaxReceipts.md)

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

# **view_specific_fax_receipt**
> ViewSpecificFaxReceipt view_specific_fax_receipt(message_id, content_type=content_type)

View Specific Fax Receipt

_Get a single fax receipt based on message id._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | path | string | true | ID of the message receipt to retrieve |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_fax_receipt import ViewSpecificFaxReceipt
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
    api_instance = clicksend.FaxOtherApi(api_client)
    message_id = 'message_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Fax Receipt
        api_response = api_instance.view_specific_fax_receipt(message_id, content_type=content_type)
        print("The response of FaxOtherApi->view_specific_fax_receipt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FaxOtherApi->view_specific_fax_receipt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificFaxReceipt**](ViewSpecificFaxReceipt.md)

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

