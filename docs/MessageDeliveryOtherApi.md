# clicksend.MessageDeliveryOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_delivery_issue**](MessageDeliveryOtherApi.md#create_delivery_issue) | **POST** /v3/delivery-issues | Create Delivery Issues
[**get_all_delivery_issues**](MessageDeliveryOtherApi.md#get_all_delivery_issues) | **GET** /v3/delivery-issues | Get All Delivery Issues


# **create_delivery_issue**
> CreateDeliveryIssue create_delivery_issue(content_type=content_type, create_delivery_issue_request=create_delivery_issue_request)

Create Delivery Issues

_Create delivery Issue_

Create delivery Issue

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| message_id | string | false | none | The message id of the message. |
| type | string | true | none | The type of message, must be one of the following values SMS, MMS, VOICE, EMAIL_MARKETING, EMAIL_TRANSACTIONAL, FAX, POST. |
| description | string | true | none | The description of the message. |
| client_comments | string | false | none | The user's comments. |
| email-address | string | true | none | The user's email address. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_delivery_issue import CreateDeliveryIssue
from clicksend.models.create_delivery_issue_request import CreateDeliveryIssueRequest
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
    api_instance = clicksend.MessageDeliveryOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_delivery_issue_request = clicksend.CreateDeliveryIssueRequest() # CreateDeliveryIssueRequest |  (optional)

    try:
        # Create Delivery Issues
        api_response = api_instance.create_delivery_issue(content_type=content_type, create_delivery_issue_request=create_delivery_issue_request)
        print("The response of MessageDeliveryOtherApi->create_delivery_issue:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageDeliveryOtherApi->create_delivery_issue: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_delivery_issue_request** | [**CreateDeliveryIssueRequest**](CreateDeliveryIssueRequest.md)|  | [optional] 

### Return type

[**CreateDeliveryIssue**](CreateDeliveryIssue.md)

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

# **get_all_delivery_issues**
> GetAllDeliveryIssues get_all_delivery_issues(content_type=content_type)

Get All Delivery Issues

_Get all delivery issues_

Get all delivery issues

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
from clicksend.models.get_all_delivery_issues import GetAllDeliveryIssues
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
    api_instance = clicksend.MessageDeliveryOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Get All Delivery Issues
        api_response = api_instance.get_all_delivery_issues(content_type=content_type)
        print("The response of MessageDeliveryOtherApi->get_all_delivery_issues:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageDeliveryOtherApi->get_all_delivery_issues: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**GetAllDeliveryIssues**](GetAllDeliveryIssues.md)

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

