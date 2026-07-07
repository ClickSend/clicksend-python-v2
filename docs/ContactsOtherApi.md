# clicksend.ContactsOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_contact**](ContactsOtherApi.md#delete_contact) | **DELETE** /v3/lists/{list_id}/contacts/{contact_id} | Delete Contact
[**get_specific_contact**](ContactsOtherApi.md#get_specific_contact) | **GET** /v3/lists/{list_id}/contacts/{contact_id} | Get Specific Contact
[**update_contact**](ContactsOtherApi.md#update_contact) | **PUT** /v3/lists/{list_id}/contacts/{contact_id} | Update Contact


# **delete_contact**
> DeleteContact delete_contact(list_id, contact_id, content_type=content_type)

Delete Contact

_Delete a contact_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List ID |
| contact_id | path | integer(int32) | true | Contact ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_contact import DeleteContact
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
    api_instance = clicksend.ContactsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Contact
        api_response = api_instance.delete_contact(list_id, contact_id, content_type=content_type)
        print("The response of ContactsOtherApi->delete_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactsOtherApi->delete_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteContact**](DeleteContact.md)

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

# **get_specific_contact**
> GetSpecificContact get_specific_contact(list_id, contact_id, content_type=content_type)

Get Specific Contact

_Get a specific contact_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your contact list id you want to access. |
| contact_id | path | integer(int32) | true | Your contact id you want to access. |


Refer to [Status
Codes](/#status-codes) for
definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_specific_contact import GetSpecificContact
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
    api_instance = clicksend.ContactsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Specific Contact
        api_response = api_instance.get_specific_contact(list_id, contact_id, content_type=content_type)
        print("The response of ContactsOtherApi->get_specific_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactsOtherApi->get_specific_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetSpecificContact**](GetSpecificContact.md)

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

# **update_contact**
> UpdateContact update_contact(list_id, contact_id, content_type=content_type, create_new_contact_request=create_new_contact_request)

Update Contact

_Update specific contact_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Contact list id |
| contact_id | path | integer(int32) | true | Contact ID |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| phone_number | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. Must be provided if no fax number or email. |
| email | string | false | none | Your email. Must be provided if no phone number or fax number. |
| fax_number | string | false | none | Your fax number. Must be provided if no phone number or email. |
| first_name | string | false | none | Your first name. |
| address_line_1 | string | false | none | Your street address |
| address_line_2 | string | false | none | none |
| address_city | string | false | none | Your nearest city |
| address_state | string | false | none | Your current state |
| address_postal_code | string | false | none | Your current postcode |
| address_country | string | false | none | Your current country |
| organization_name | string | false | none | Your organisation name |
| custom_1 | string | true | none | none |
| custom_2 | string | false | none | none |
| custom_3 | string | false | none | none |
| custom_4 | string | false | none | none |
| last_name | string | false | none | Your last name |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_new_contact_request import CreateNewContactRequest
from clicksend.models.update_contact import UpdateContact
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
    api_instance = clicksend.ContactsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_new_contact_request = clicksend.CreateNewContactRequest() # CreateNewContactRequest |  (optional)

    try:
        # Update Contact
        api_response = api_instance.update_contact(list_id, contact_id, content_type=content_type, create_new_contact_request=create_new_contact_request)
        print("The response of ContactsOtherApi->update_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContactsOtherApi->update_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_new_contact_request** | [**CreateNewContactRequest**](CreateNewContactRequest.md)|  | [optional] 

### Return type

[**UpdateContact**](UpdateContact.md)

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

