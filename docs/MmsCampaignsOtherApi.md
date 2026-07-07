# clicksend.MmsCampaignsOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_mms_campaign_price**](MmsCampaignsOtherApi.md#calculate_mms_campaign_price) | **POST** /v3/mms-campaigns/price | Calculate MMS Campaign Price
[**cancel_mms_campaign**](MmsCampaignsOtherApi.md#cancel_mms_campaign) | **PUT** /v3/mms-campaigns/{mms_campaign_id}/cancel | Cancel MMS Campaign
[**send_mms_campaign**](MmsCampaignsOtherApi.md#send_mms_campaign) | **POST** /v3/mms-campaigns/send | Send MMS Campaign
[**update_mms_campaign**](MmsCampaignsOtherApi.md#update_mms_campaign) | **PUT** /v3/mms-campaigns/{mms_campaign_id} | Update MMS Campaign
[**view_all_mms_campaigns**](MmsCampaignsOtherApi.md#view_all_mms_campaigns) | **GET** /v3/mms-campaigns | View All MMS Campaigns
[**view_mms_campaign**](MmsCampaignsOtherApi.md#view_mms_campaign) | **GET** /v3/mms-campaigns/{mms_campaign_id} | View MMS Campaign


# **calculate_mms_campaign_price**
> CalculateMmsCampaignPrice calculate_mms_campaign_price(content_type=content_type, body=body)

Calculate MMS Campaign Price

_Calculate price for mms campaign_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |
| subject | string | true | none | Subject of MMS campaign. |
| media_file | string | true | none | URL pointing to media file. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_mms_campaign_price import CalculateMmsCampaignPrice
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
    api_instance = clicksend.MmsCampaignsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Calculate MMS Campaign Price
        api_response = api_instance.calculate_mms_campaign_price(content_type=content_type, body=body)
        print("The response of MmsCampaignsOtherApi->calculate_mms_campaign_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsCampaignsOtherApi->calculate_mms_campaign_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CalculateMmsCampaignPrice**](CalculateMmsCampaignPrice.md)

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

# **cancel_mms_campaign**
> CancelMmsCampaign cancel_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Cancel MMS Campaign

_Cancel mms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| mms_campaign_id | path | integer(int32) | true | ID of MMS Campaign to cancel |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
from clicksend.models.cancel_mms_campaign import CancelMmsCampaign
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
    api_instance = clicksend.MmsCampaignsOtherApi(api_client)
    mms_campaign_id = 'mms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Cancel MMS Campaign
        api_response = api_instance.cancel_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of MmsCampaignsOtherApi->cancel_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsCampaignsOtherApi->cancel_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**CancelMmsCampaign**](CancelMmsCampaign.md)

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

# **send_mms_campaign**
> SendMmsCampaign send_mms_campaign(content_type=content_type, send_mms_campaign_request=send_mms_campaign_request)

Send MMS Campaign

_Create mms campaign_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |
| subject | string | true | none | Subject of MMS campaign. |
| media_file | string | true | none | URL pointing to media file. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_mms_campaign import SendMmsCampaign
from clicksend.models.send_mms_campaign_request import SendMmsCampaignRequest
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
    api_instance = clicksend.MmsCampaignsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_mms_campaign_request = clicksend.SendMmsCampaignRequest() # SendMmsCampaignRequest |  (optional)

    try:
        # Send MMS Campaign
        api_response = api_instance.send_mms_campaign(content_type=content_type, send_mms_campaign_request=send_mms_campaign_request)
        print("The response of MmsCampaignsOtherApi->send_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsCampaignsOtherApi->send_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_mms_campaign_request** | [**SendMmsCampaignRequest**](SendMmsCampaignRequest.md)|  | [optional] 

### Return type

[**SendMmsCampaign**](SendMmsCampaign.md)

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

# **update_mms_campaign**
> UpdateMmsCampaign update_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Update MMS Campaign

_Update mms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| mms_campaign_id | path | integer(int32) | true | ID of MMS campaign to update |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |
| subject | string | true | none | Subject of MMS campaign. |
| media_file | string | true | none | URL pointing to media file. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
from clicksend.models.update_mms_campaign import UpdateMmsCampaign
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
    api_instance = clicksend.MmsCampaignsOtherApi(api_client)
    mms_campaign_id = 'mms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Update MMS Campaign
        api_response = api_instance.update_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of MmsCampaignsOtherApi->update_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsCampaignsOtherApi->update_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**UpdateMmsCampaign**](UpdateMmsCampaign.md)

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

# **view_all_mms_campaigns**
> ViewAllMmsCampaigns view_all_mms_campaigns(content_type=content_type)

View All MMS Campaigns

_Get list of mms campaigns_

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
from clicksend.models.view_all_mms_campaigns import ViewAllMmsCampaigns
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
    api_instance = clicksend.MmsCampaignsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View All MMS Campaigns
        api_response = api_instance.view_all_mms_campaigns(content_type=content_type)
        print("The response of MmsCampaignsOtherApi->view_all_mms_campaigns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsCampaignsOtherApi->view_all_mms_campaigns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllMmsCampaigns**](ViewAllMmsCampaigns.md)

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

# **view_mms_campaign**
> ViewMmsCampaign view_mms_campaign(mms_campaign_id, content_type=content_type)

View MMS Campaign

_Get specific mms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| mms_campaign_id | path | integer(int32) | true | ID of MMS campaign to retrieve |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_mms_campaign import ViewMmsCampaign
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
    api_instance = clicksend.MmsCampaignsOtherApi(api_client)
    mms_campaign_id = 'mms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View MMS Campaign
        api_response = api_instance.view_mms_campaign(mms_campaign_id, content_type=content_type)
        print("The response of MmsCampaignsOtherApi->view_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MmsCampaignsOtherApi->view_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewMmsCampaign**](ViewMmsCampaign.md)

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

