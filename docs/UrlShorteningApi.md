# clicksend.UrlShorteningApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**short_url_get_statistics**](UrlShorteningApi.md#short_url_get_statistics) | **GET** /v3/short-url/statistics/{source}/{source_id} | Get Statistics
[**short_url_get_tracking**](UrlShorteningApi.md#short_url_get_tracking) | **GET** /v3/short-url/tracking/{long_url_id} | Get Tracking


# **short_url_get_statistics**
> GetStatistics short_url_get_statistics(source, source_id, content_type=content_type)

Get Statistics

Use this endpoint to get the aggregated statistics for a shortened URL. This allows you to track the total number of clicks on the link. You can gather details such as the device type and where it was opened from as well.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_statistics import GetStatistics
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
    api_instance = clicksend.UrlShorteningApi(api_client)
    source = 'source_example' # str | Source of the request.
    source_id = 'source_id_example' # str | ID of the source (e.g. message ID).
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Statistics
        api_response = api_instance.short_url_get_statistics(source, source_id, content_type=content_type)
        print("The response of UrlShorteningApi->short_url_get_statistics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UrlShorteningApi->short_url_get_statistics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **source** | **str**| Source of the request. | 
 **source_id** | **str**| ID of the source (e.g. message ID). | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetStatistics**](GetStatistics.md)

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

# **short_url_get_tracking**
> GetTracking short_url_get_tracking(long_url_id, content_type=content_type)

Get Tracking

Use this endpoint to track how individual recipients interact with the link.  It returns data from the most recent click, including statistics such as how many times they’ve visited the link and when it was last opened. To use this endpoint, reference the _long_url_id_ provided in the [GET /short-url/statistics](/messaging/url-shortening/other/short-url-get-statistics) endpoint.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_tracking import GetTracking
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
    api_instance = clicksend.UrlShorteningApi(api_client)
    long_url_id = 'long_url_id_example' # str | ID of the long URL (uniquely defined by the source, source ID, and long URL). Obtained from the GET statistics endpoint.
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Tracking
        api_response = api_instance.short_url_get_tracking(long_url_id, content_type=content_type)
        print("The response of UrlShorteningApi->short_url_get_tracking:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UrlShorteningApi->short_url_get_tracking: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **long_url_id** | **str**| ID of the long URL (uniquely defined by the source, source ID, and long URL). Obtained from the GET statistics endpoint. | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetTracking**](GetTracking.md)

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

