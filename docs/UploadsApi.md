# clicksend.UploadsApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**upload_a_media_file**](UploadsApi.md#upload_a_media_file) | **POST** /v3/uploads | Upload Media File


# **upload_a_media_file**
> upload_a_media_file(content_type=content_type, body=body)

Upload Media File

The `upload` endpoint provides a method for converting files from an unsupported format to a format that one of our endpoints can handle.

Files can be submitted two ways: 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`\-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string. 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.

Note that `convert` specifies the conversion to take place. That is, what the result should be compatible with and can be any of the following:

- `fax`
- `mms`
- `csv`
- `post`
- `postcard`
    

All files will expire 10 minutes after being uploaded.

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| convert | query | string | true | none |
| content | body | string | true | Base64-encoded file contents |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

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
    api_instance = clicksend.UploadsApi(api_client)
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Upload Media File
        api_instance.upload_a_media_file(content_type=content_type, body=body)
    except Exception as e:
        print("Exception when calling UploadsApi->upload_a_media_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

void (empty response body)

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

