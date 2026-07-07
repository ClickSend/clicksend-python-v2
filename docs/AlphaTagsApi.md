# clicksend.AlphaTagsApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_alpha_tag**](AlphaTagsApi.md#delete_alpha_tag) | **DELETE** /v3/alpha-tags/{alpha_tag_id} | Delete Alpha Tag
[**get_alpha_tag**](AlphaTagsApi.md#get_alpha_tag) | **GET** /v3/alpha-tags/{alpha_tag_id} | Get Alpha Tag
[**list_alpha_tags**](AlphaTagsApi.md#list_alpha_tags) | **GET** /v3/alpha-tags | List Alpha Tags
[**request_alpha_tag**](AlphaTagsApi.md#request_alpha_tag) | **POST** /v3/alpha-tags | Request Alpha Tag


# **delete_alpha_tag**
> delete_alpha_tag(alpha_tag_id, content_type=content_type)

Delete Alpha Tag

_Delete a specific alpha tag._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| alpha_tag_id | path | uuid | true | ID of the alpha tag |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

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
    api_instance = clicksend.AlphaTagsApi(api_client)
    alpha_tag_id = 'alpha_tag_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Alpha Tag
        api_instance.delete_alpha_tag(alpha_tag_id, content_type=content_type)
    except Exception as e:
        print("Exception when calling AlphaTagsApi->delete_alpha_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **alpha_tag_id** | **str**|  | 
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

# **get_alpha_tag**
> AlphaTag get_alpha_tag(alpha_tag_id, content_type=content_type)

Get Alpha Tag

_Get a specific alpha tag._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| alpha_tag_id | path | uuid | true | ID of the alpha tag |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

 This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.alpha_tag import AlphaTag
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
    api_instance = clicksend.AlphaTagsApi(api_client)
    alpha_tag_id = 'alpha_tag_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Alpha Tag
        api_response = api_instance.get_alpha_tag(alpha_tag_id, content_type=content_type)
        print("The response of AlphaTagsApi->get_alpha_tag:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlphaTagsApi->get_alpha_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **alpha_tag_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**AlphaTag**](AlphaTag.md)

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

# **list_alpha_tags**
> ListAlphaTags list_alpha_tags(sort_direction=sort_direction, page_size=page_size)

List Alpha Tags



### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_alpha_tags import ListAlphaTags
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
    api_instance = clicksend.AlphaTagsApi(api_client)
    sort_direction = asc # str | The sort direction for the results. The default value is asc. (optional) (default to asc)
    page_size = 10 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 10. (optional) (default to 10)

    try:
        # List Alpha Tags
        api_response = api_instance.list_alpha_tags(sort_direction=sort_direction, page_size=page_size)
        print("The response of AlphaTagsApi->list_alpha_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlphaTagsApi->list_alpha_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sort_direction** | **str**| The sort direction for the results. The default value is asc. | [optional] [default to asc]
 **page_size** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 10. | [optional] [default to 10]

### Return type

[**ListAlphaTags**](ListAlphaTags.md)

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

# **request_alpha_tag**
> AlphaTag request_alpha_tag(content_type=content_type, request_alpha_tag_request=request_alpha_tag_request)

Request Alpha Tag

_Request to register an alpha tag. After requested, the alpha tag will be reviewed by ClickSend and either approved or rejected. Some countries (e.g Australia) require you to submit additional fields due to government mandated compliance checks._

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| alpha_tag | string | true | [yes](https://help.clicksend.com/article/1qxfxkcwm2-global-generic-alpha-tags) | The alpha tag name. Length must be between 3 - 11 characters, can only contain a-z A-Z 0-9 + and must contain at least one non numeric. |
| reason | string | false | none | Must be one of the following: `Sole Trader Name`, `Company Name`, `Partnership Name`, `Registered Trust Name`, `Co-Operative Name`, `Indigenous Corporation Name`, `Registered Organisation Name`, `Personal Name`, `Trademark`, `Government Agency or Entity`, `Product or Service Name`, `Acronym/Initialism`, `Contraction of Name`, `Third Party`. In case of `Third Party`, we will contact you to collect the relevant information. |
| countries | array of strings | false | none | List of country codes (e.g., "AU", "US") where the alpha tag is requested. Only supported and required for AU. |
| businesses | array of objects | false | none | List of business details required for alpha tag registration. Each object contains country, business information, ... Required if `countries` is provided. When `business_relationship` is `ENTITY_ASSOCIATE`, the following partner fields are also **required**: `partner_business_name`, `partner_abn`, `partner_business_info`, `partner_business_address`, `partner_representative`. These fields are **forbidden** for any other `business_relationship` value. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

_This endpoint requires authentication,_ [more info...](/#authentication)


### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.alpha_tag import AlphaTag
from clicksend.models.request_alpha_tag_request import RequestAlphaTagRequest
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
    api_instance = clicksend.AlphaTagsApi(api_client)
    content_type = 'application/json' # str |  (optional)
    request_alpha_tag_request = {"alpha_tag":"MyCompany","reason":"Company Name"} # RequestAlphaTagRequest |  (optional)

    try:
        # Request Alpha Tag
        api_response = api_instance.request_alpha_tag(content_type=content_type, request_alpha_tag_request=request_alpha_tag_request)
        print("The response of AlphaTagsApi->request_alpha_tag:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlphaTagsApi->request_alpha_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **request_alpha_tag_request** | [**RequestAlphaTagRequest**](RequestAlphaTagRequest.md)|  | [optional] 

### Return type

[**AlphaTag**](AlphaTag.md)

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

