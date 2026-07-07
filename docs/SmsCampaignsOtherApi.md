# clicksend.SmsCampaignsOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calculate_sms_campaign_price**](SmsCampaignsOtherApi.md#calculate_sms_campaign_price) | **POST** /v3/sms-campaigns/price | Calculate SMS Campaign Price
[**cancel_sms_campaign**](SmsCampaignsOtherApi.md#cancel_sms_campaign) | **PUT** /v3/sms-campaigns/{sms_campaign_id}/cancel | Cancel SMS Campaign
[**send_sms_campaign**](SmsCampaignsOtherApi.md#send_sms_campaign) | **POST** /v3/sms-campaigns/send | Send SMS Campaign
[**update_sms_campaign**](SmsCampaignsOtherApi.md#update_sms_campaign) | **PUT** /v3/sms-campaigns/{sms_campaign_id} | Update SMS Campaign
[**view_sms_campaigns**](SmsCampaignsOtherApi.md#view_sms_campaigns) | **GET** /v3/sms-campaigns | View SMS Campaigns
[**view_specific_sms_campaign**](SmsCampaignsOtherApi.md#view_specific_sms_campaign) | **GET** /v3/sms-campaigns/{sms_campaign_id} | View Specific SMS Campaign


# **calculate_sms_campaign_price**
> CalculateSmsCampaignPrice calculate_sms_campaign_price(content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Calculate SMS Campaign Price

_Calculate price for sms campaign_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
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
from clicksend.models.calculate_sms_campaign_price import CalculateSmsCampaignPrice
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
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
    api_instance = clicksend.SmsCampaignsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Calculate SMS Campaign Price
        api_response = api_instance.calculate_sms_campaign_price(content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of SmsCampaignsOtherApi->calculate_sms_campaign_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsCampaignsOtherApi->calculate_sms_campaign_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**CalculateSmsCampaignPrice**](CalculateSmsCampaignPrice.md)

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

# **cancel_sms_campaign**
> CancelSmsCampaign cancel_sms_campaign(sms_campaign_id, content_type=content_type)

Cancel SMS Campaign

Use this endpoint to cancel a scheduled SMS campaign.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_sms_campaign import CancelSmsCampaign
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
    api_instance = clicksend.SmsCampaignsOtherApi(api_client)
    sms_campaign_id = 'sms_campaign_id_example' # str | ID of the scheduled SMS campaign to cancel.
    content_type = 'application/json' # str |  (optional)

    try:
        # Cancel SMS Campaign
        api_response = api_instance.cancel_sms_campaign(sms_campaign_id, content_type=content_type)
        print("The response of SmsCampaignsOtherApi->cancel_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsCampaignsOtherApi->cancel_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_campaign_id** | **str**| ID of the scheduled SMS campaign to cancel. | 
 **content_type** | **str**|  | [optional] 

### Return type

[**CancelSmsCampaign**](CancelSmsCampaign.md)

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

# **send_sms_campaign**
> SendSmsCampaign send_sms_campaign(content_type=content_type, send_sms_campaign_request=send_sms_campaign_request)

Send SMS Campaign

### _SMS Campaign Endpoint_

You can post to a list with `up to 20000 recipients` with each API call. You can only send to a single list containing up to 20,000 recipients. The response is far less detailed than the normal Send SMS endpoint. Use the [SMS Send](/#send-sms) endpoint if you would like to send to less than 1000 recipients at once.
You are required to add an opt-out message to the end of your message body if you are sending marketing message. This can be in the form of asking users to reply STOP to opt-out or by including `StopMsg.me/xxxxx` which is a placeholder that will add a link that can be clicked to out-out.
Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.
<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_sms_campaign import SendSmsCampaign
from clicksend.models.send_sms_campaign_request import SendSmsCampaignRequest
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
    api_instance = clicksend.SmsCampaignsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_sms_campaign_request = clicksend.SendSmsCampaignRequest() # SendSmsCampaignRequest |  (optional)

    try:
        # Send SMS Campaign
        api_response = api_instance.send_sms_campaign(content_type=content_type, send_sms_campaign_request=send_sms_campaign_request)
        print("The response of SmsCampaignsOtherApi->send_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsCampaignsOtherApi->send_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_sms_campaign_request** | [**SendSmsCampaignRequest**](SendSmsCampaignRequest.md)|  | [optional] 

### Return type

[**SendSmsCampaign**](SendSmsCampaign.md)

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

# **update_sms_campaign**
> UpdateSmsCampaign update_sms_campaign(sms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Update SMS Campaign

_Update sms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| sms_campaign_id | path | integer(int32) | true | ID of SMS campaign to update |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
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
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
from clicksend.models.update_sms_campaign import UpdateSmsCampaign
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
    api_instance = clicksend.SmsCampaignsOtherApi(api_client)
    sms_campaign_id = 'sms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Update SMS Campaign
        api_response = api_instance.update_sms_campaign(sms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of SmsCampaignsOtherApi->update_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsCampaignsOtherApi->update_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**UpdateSmsCampaign**](UpdateSmsCampaign.md)

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

# **view_sms_campaigns**
> ViewSmsCampaigns view_sms_campaigns(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)

View SMS Campaigns

Use this endpoint to view SMS campaigns.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_campaigns import ViewSmsCampaigns
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
    api_instance = clicksend.SmsCampaignsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | The page number to retrieve. Use this parameter to navigate through the [pagination]/#pagination) results. The default value is 1. (optional) (default to 1)
    limit = 15 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
    q = 'q_example' # str | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS campaign you want to filter by. You can use the following fields:      - sms_campaign_id,name,user_id,subaccount_id,list_id,from,body,schedule,status,date_added,custom_string,url_to_shorten,unsubscribe_link,source   2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.  For example, if you are searching for a SMS campaign with the status of _Scheduled_, the final query would look like this:    - `q=status:Scheduled`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>   Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/>    <ul>     <li>q=from:%2B61437085284</li>   </ul>    You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.      </p> </div> (optional)
    order_by = 'order_by_example' # str | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_added_ in ascending order. You can use the following fields:    - _name_: The name of the SMS campaign.   - _status_: The status of the SMS campaign.   - _schedule_: The schedule send date of the SMS campaign in the <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>.   - _from_: The sender of the SMS campaign.   - _date_added_: This is the date you created or updated the SMS campaign in the <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>.  For example, if you want to order by the most recently sent or scheduled SMS, you should sort by date in descending order. The query would look like this:    - `order_by=schedule:desc`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>     You can also sort by these fields: <br/>     <ul>     <li>sms_campaign_id,user_id,subaccount_id,list_id,body,custom_string,url_to_shorten,unsubscribe_link, and source.</li>   </ul>   <br/>   But this is less common in practice.   </p> </div> (optional)
    date_from = 56 # int | Start date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)
    date_to = 56 # int | End date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)

    try:
        # View SMS Campaigns
        api_response = api_instance.view_sms_campaigns(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)
        print("The response of SmsCampaignsOtherApi->view_sms_campaigns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsCampaignsOtherApi->view_sms_campaigns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| The page number to retrieve. Use this parameter to navigate through the [pagination]/#pagination) results. The default value is 1. | [optional] [default to 1]
 **limit** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [optional] [default to 15]
 **q** | **str**| Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS campaign you want to filter by. You can use the following fields:      - sms_campaign_id,name,user_id,subaccount_id,list_id,from,body,schedule,status,date_added,custom_string,url_to_shorten,unsubscribe_link,source   2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.  For example, if you are searching for a SMS campaign with the status of _Scheduled_, the final query would look like this:    - &#x60;q&#x3D;status:Scheduled&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;   Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;    &lt;ul&gt;     &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;   &lt;/ul&gt;    You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.      &lt;/p&gt; &lt;/div&gt; | [optional] 
 **order_by** | **str**| Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_added_ in ascending order. You can use the following fields:    - _name_: The name of the SMS campaign.   - _status_: The status of the SMS campaign.   - _schedule_: The schedule send date of the SMS campaign in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;.   - _from_: The sender of the SMS campaign.   - _date_added_: This is the date you created or updated the SMS campaign in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;.  For example, if you want to order by the most recently sent or scheduled SMS, you should sort by date in descending order. The query would look like this:    - &#x60;order_by&#x3D;schedule:desc&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;     You can also sort by these fields: &lt;br/&gt;     &lt;ul&gt;     &lt;li&gt;sms_campaign_id,user_id,subaccount_id,list_id,body,custom_string,url_to_shorten,unsubscribe_link, and source.&lt;/li&gt;   &lt;/ul&gt;   &lt;br/&gt;   But this is less common in practice.   &lt;/p&gt; &lt;/div&gt; | [optional] 
 **date_from** | **int**| Start date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
 **date_to** | **int**| End date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 

### Return type

[**ViewSmsCampaigns**](ViewSmsCampaigns.md)

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

# **view_specific_sms_campaign**
> ViewSpecificSmsCampaign view_specific_sms_campaign(sms_campaign_id, content_type=content_type)

View Specific SMS Campaign

Use this endpoint to view a specific SMS campaign.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_sms_campaign import ViewSpecificSmsCampaign
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
    api_instance = clicksend.SmsCampaignsOtherApi(api_client)
    sms_campaign_id = 'sms_campaign_id_example' # str | ID of SMS campaign to get
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific SMS Campaign
        api_response = api_instance.view_specific_sms_campaign(sms_campaign_id, content_type=content_type)
        print("The response of SmsCampaignsOtherApi->view_specific_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SmsCampaignsOtherApi->view_specific_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_campaign_id** | **str**| ID of SMS campaign to get | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificSmsCampaign**](ViewSpecificSmsCampaign.md)

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

