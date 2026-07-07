# clicksend.ReferralsApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**view_referral_accounts**](ReferralsApi.md#view_referral_accounts) | **GET** /v3/referral/accounts/ | View Referral Accounts


# **view_referral_accounts**
> ViewReferralAccounts view_referral_accounts(content_type=content_type)

View Referral Accounts

_Get all referral accounts_

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
from clicksend.models.view_referral_accounts import ViewReferralAccounts
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
    api_instance = clicksend.ReferralsApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Referral Accounts
        api_response = api_instance.view_referral_accounts(content_type=content_type)
        print("The response of ReferralsApi->view_referral_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReferralsApi->view_referral_accounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewReferralAccounts**](ViewReferralAccounts.md)

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

