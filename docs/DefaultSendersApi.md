# clicksend.DefaultSendersApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_default_sender**](DefaultSendersApi.md#create_default_sender) | **POST** /v3/senders/default-senders | Create Default Sender
[**delete_default_sender**](DefaultSendersApi.md#delete_default_sender) | **DELETE** /v3/senders/default-senders/{default_sender_id} | Delete Default Sender
[**get_default_sender_details**](DefaultSendersApi.md#get_default_sender_details) | **GET** /v3/senders/default-senders/{default_sender_id} | Get Default Sender Details
[**get_default_senders_list**](DefaultSendersApi.md#get_default_senders_list) | **GET** /v3/senders/default-senders | Get List of Default Senders
[**list_compliant_sender_types**](DefaultSendersApi.md#list_compliant_sender_types) | **GET** /v3/senders/compliant-sender-types | List Compliant Sender Types
[**update_default_sender**](DefaultSendersApi.md#update_default_sender) | **PATCH** /v3/senders/default-senders/{default_sender_id} | Update Default Sender


# **create_default_sender**
> CreateDefaultSender create_default_sender(content_type=content_type, create_default_sender_request=create_default_sender_request)

Create Default Sender

Creates a new default sender configuration to automate the selection of compliant SenderIDs.
By configuring a default sender you no longer need to define the `sender_id` string when sending SMS messages. The default sender will be picked up automatically.

For more information on Sender IDs, please refer to [What is a Sender ID or Sender Number?](https://help.clicksend.com/article/4kgj7krx00-what-is-a-sender-id-or-sender-number)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_default_sender import CreateDefaultSender
from clicksend.models.create_default_sender_request import CreateDefaultSenderRequest
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
    api_instance = clicksend.DefaultSendersApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_default_sender_request = clicksend.CreateDefaultSenderRequest() # CreateDefaultSenderRequest |  (optional)

    try:
        # Create Default Sender
        api_response = api_instance.create_default_sender(content_type=content_type, create_default_sender_request=create_default_sender_request)
        print("The response of DefaultSendersApi->create_default_sender:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultSendersApi->create_default_sender: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_default_sender_request** | [**CreateDefaultSenderRequest**](CreateDefaultSenderRequest.md)|  | [optional] 

### Return type

[**CreateDefaultSender**](CreateDefaultSender.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**400** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_default_sender**
> delete_default_sender(default_sender_id, content_type=content_type)

Delete Default Sender

Removes a specified default sender setting. 
If you don't configure a default sender and leave the `sender_id` string blank when sending an SMS,
Smart Assign will pick the best suitable, compliant, available SenderID for you.

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
    api_instance = clicksend.DefaultSendersApi(api_client)
    default_sender_id = 'default_sender_id_example' # str | The ID of the default sender to delete
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Default Sender
        api_instance.delete_default_sender(default_sender_id, content_type=content_type)
    except Exception as e:
        print("Exception when calling DefaultSendersApi->delete_default_sender: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **default_sender_id** | **str**| The ID of the default sender to delete | 
 **content_type** | **str**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Successful response (No Content) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_default_sender_details**
> GetDefaultSenderDetails get_default_sender_details(default_sender_id, content_type=content_type)

Get Default Sender Details

Retrieve detailed information about a specific default sender configuration

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_default_sender_details import GetDefaultSenderDetails
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
    api_instance = clicksend.DefaultSendersApi(api_client)
    default_sender_id = 'default_sender_id_example' # str | The ID of the default sender to retrieve
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Default Sender Details
        api_response = api_instance.get_default_sender_details(default_sender_id, content_type=content_type)
        print("The response of DefaultSendersApi->get_default_sender_details:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultSendersApi->get_default_sender_details: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **default_sender_id** | **str**| The ID of the default sender to retrieve | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetDefaultSenderDetails**](GetDefaultSenderDetails.md)

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

# **get_default_senders_list**
> GetDefaultSendersList get_default_senders_list(content_type=content_type, offset=offset, per_page=per_page, sort_by=sort_by, sort_direction=sort_direction)

Get List of Default Senders

Retrieve a list of default senders for the current user

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_default_senders_list import GetDefaultSendersList
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
    api_instance = clicksend.DefaultSendersApi(api_client)
    content_type = 'application/json' # str |  (optional)
    offset = 'offset_example' # str | Page (offset) to be used for pagination (optional)
    per_page = 10 # int | Size of the page in pagination (optional) (default to 10)
    sort_by = 'created_timestamp' # str | Parameter to sort the results by (optional) (default to 'created_timestamp')
    sort_direction = desc # str | Direction of sorting (optional) (default to desc)

    try:
        # Get List of Default Senders
        api_response = api_instance.get_default_senders_list(content_type=content_type, offset=offset, per_page=per_page, sort_by=sort_by, sort_direction=sort_direction)
        print("The response of DefaultSendersApi->get_default_senders_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultSendersApi->get_default_senders_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **offset** | **str**| Page (offset) to be used for pagination | [optional] 
 **per_page** | **int**| Size of the page in pagination | [optional] [default to 10]
 **sort_by** | **str**| Parameter to sort the results by | [optional] [default to &#39;created_timestamp&#39;]
 **sort_direction** | **str**| Direction of sorting | [optional] [default to desc]

### Return type

[**GetDefaultSendersList**](GetDefaultSendersList.md)

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

# **list_compliant_sender_types**
> ListCompliantSenderTypes200Response list_compliant_sender_types(filter_product_type, filter_country_code_index=filter_country_code_index)

List Compliant Sender Types

Retrieves the list of compliant sender types for specific countries

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_compliant_sender_types200_response import ListCompliantSenderTypes200Response
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
    api_instance = clicksend.DefaultSendersApi(api_client)
    filter_product_type = 'SMS' # str | Type of the product
    filter_country_code_index = ['filter_country_code_index_example'] # List[str] | Array of recipient country codes (ISO 3166-1 alpha-2). If not specified, will get all compliant sender types for all countries. Replace `{index}` with the appropriate index value.  <small>Example:</small> <small><code style=\"color: #424242;\">filter[country_code][0]=US&filter[country_code][1]=AU</code></small>  (optional)

    try:
        # List Compliant Sender Types
        api_response = api_instance.list_compliant_sender_types(filter_product_type, filter_country_code_index=filter_country_code_index)
        print("The response of DefaultSendersApi->list_compliant_sender_types:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultSendersApi->list_compliant_sender_types: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_product_type** | **str**| Type of the product | 
 **filter_country_code_index** | [**List[str]**](str.md)| Array of recipient country codes (ISO 3166-1 alpha-2). If not specified, will get all compliant sender types for all countries. Replace &#x60;{index}&#x60; with the appropriate index value.  &lt;small&gt;Example:&lt;/small&gt; &lt;small&gt;&lt;code style&#x3D;\&quot;color: #424242;\&quot;&gt;filter[country_code][0]&#x3D;US&amp;filter[country_code][1]&#x3D;AU&lt;/code&gt;&lt;/small&gt;  | [optional] 

### Return type

[**ListCompliantSenderTypes200Response**](ListCompliantSenderTypes200Response.md)

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

# **update_default_sender**
> UpdateDefaultSender update_default_sender(default_sender_id, content_type=content_type, update_default_sender_request=update_default_sender_request)

Update Default Sender

Updates the details of an existing default sender configuration.

For more information on Sender IDs, please refer to [What is a Sender ID or Sender Number?](https://help.clicksend.com/article/4kgj7krx00-what-is-a-sender-id-or-sender-number)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_default_sender import UpdateDefaultSender
from clicksend.models.update_default_sender_request import UpdateDefaultSenderRequest
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
    api_instance = clicksend.DefaultSendersApi(api_client)
    default_sender_id = 'default_sender_id_example' # str | The ID of the default sender to update
    content_type = 'application/json' # str |  (optional)
    update_default_sender_request = clicksend.UpdateDefaultSenderRequest() # UpdateDefaultSenderRequest |  (optional)

    try:
        # Update Default Sender
        api_response = api_instance.update_default_sender(default_sender_id, content_type=content_type, update_default_sender_request=update_default_sender_request)
        print("The response of DefaultSendersApi->update_default_sender:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultSendersApi->update_default_sender: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **default_sender_id** | **str**| The ID of the default sender to update | 
 **content_type** | **str**|  | [optional] 
 **update_default_sender_request** | [**UpdateDefaultSenderRequest**](UpdateDefaultSenderRequest.md)|  | [optional] 

### Return type

[**UpdateDefaultSender**](UpdateDefaultSender.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

