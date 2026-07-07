# clicksend.ListsOtherApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**copy_contact_to_list**](ListsOtherApi.md#copy_contact_to_list) | **PUT** /v3/lists/{from_list_id}/contacts/{contact_id}/copy/{to_list_id} | Copy Contact to List
[**create_list**](ListsOtherApi.md#create_list) | **POST** /v3/lists | Create List
[**create_new_contact**](ListsOtherApi.md#create_new_contact) | **POST** /v3/lists/{list_id}/contacts | Create New Contact
[**delete_list**](ListsOtherApi.md#delete_list) | **DELETE** /v3/lists/{list_id} | Delete List
[**import_contacts**](ListsOtherApi.md#import_contacts) | **POST** /v3/lists/{list_id}/import | Import Contacts
[**remove_duplicate_contacts**](ListsOtherApi.md#remove_duplicate_contacts) | **PUT** /v3/lists/{list_id}/remove-duplicates/ | Remove Duplicate Contacts
[**remove_opted_out_contacts**](ListsOtherApi.md#remove_opted_out_contacts) | **PUT** /v3/lists/{list_id}/remove-opted-out-contacts/{opt_out_list_id} | Remove Opted Out Contacts
[**transfer_contact_to_list**](ListsOtherApi.md#transfer_contact_to_list) | **PUT** /v3/lists/{from_list_id}/contacts/{contact_id}/transfer/{to_list_id} | Transfer Contact to List
[**update_list**](ListsOtherApi.md#update_list) | **PUT** /v3/lists/{list_id} | Update List
[**view_contact_lists**](ListsOtherApi.md#view_contact_lists) | **GET** /v3/search/contacts-lists | View Contact Lists
[**view_list_contacts**](ListsOtherApi.md#view_list_contacts) | **GET** /v3/lists/{list_id}/contacts | View List Contacts
[**view_lists**](ListsOtherApi.md#view_lists) | **GET** /v3/lists | View Lists
[**view_specific_list**](ListsOtherApi.md#view_specific_list) | **GET** /v3/lists/{list_id} | View Specific List


# **copy_contact_to_list**
> CopyContactToList copy_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)

Copy Contact to List

_Copy contact to another list_

Copy contact to another list

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| from_list_id | path | integer(int32) | true | List ID for list that contains contact. |
| contact_id | path | integer(int32) | true | Contact ID |
| to_list_id | path | integer(int32) | true | List ID for list you want to copy contact to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.copy_contact_to_list import CopyContactToList
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
    api_instance = clicksend.ListsOtherApi(api_client)
    from_list_id = 'from_list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    to_list_id = 'to_list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Copy Contact to List
        api_response = api_instance.copy_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)
        print("The response of ListsOtherApi->copy_contact_to_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->copy_contact_to_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from_list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **to_list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CopyContactToList**](CopyContactToList.md)

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

# **create_list**
> CreateList create_list(content_type=content_type, create_list_request=create_list_request)

Create List

_Create new contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_name | body | string | true | Your contact list name |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_list import CreateList
from clicksend.models.create_list_request import CreateListRequest
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
    api_instance = clicksend.ListsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_list_request = clicksend.CreateListRequest() # CreateListRequest |  (optional)

    try:
        # Create List
        api_response = api_instance.create_list(content_type=content_type, create_list_request=create_list_request)
        print("The response of ListsOtherApi->create_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->create_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_list_request** | [**CreateListRequest**](CreateListRequest.md)|  | [optional] 

### Return type

[**CreateList**](CreateList.md)

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

# **create_new_contact**
> CreateNewContact create_new_contact(list_id, content_type=content_type, create_new_contact_request=create_new_contact_request)

Create New Contact

_Create new contact_

### parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List id |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| phone_number | string | true | none | Your phone number in\_[E.164](https://en.wikipedia.org/wiki/E.164)\_format. Must be provided if no fax number or email. |
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
from clicksend.models.create_new_contact import CreateNewContact
from clicksend.models.create_new_contact_request import CreateNewContactRequest
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_new_contact_request = clicksend.CreateNewContactRequest() # CreateNewContactRequest |  (optional)

    try:
        # Create New Contact
        api_response = api_instance.create_new_contact(list_id, content_type=content_type, create_new_contact_request=create_new_contact_request)
        print("The response of ListsOtherApi->create_new_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->create_new_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_new_contact_request** | [**CreateNewContactRequest**](CreateNewContactRequest.md)|  | [optional] 

### Return type

[**CreateNewContact**](CreateNewContact.md)

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

# **delete_list**
> DeleteList delete_list(list_id, content_type=content_type)

Delete List

_ListsByListIdDelete_

Delete a specific contact list

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List ID |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_list import DeleteList
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete List
        api_response = api_instance.delete_list(list_id, content_type=content_type)
        print("The response of ListsOtherApi->delete_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->delete_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteList**](DeleteList.md)

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

# **import_contacts**
> ImportContacts import_contacts(list_id, content_type=content_type, import_contacts_request=import_contacts_request)

Import Contacts

_Import contacts to list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your contact list id you want to access. |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to process |
| field_order | \[string\] | true | none | Order of fields in file |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.import_contacts import ImportContacts
from clicksend.models.import_contacts_request import ImportContactsRequest
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    import_contacts_request = clicksend.ImportContactsRequest() # ImportContactsRequest |  (optional)

    try:
        # Import Contacts
        api_response = api_instance.import_contacts(list_id, content_type=content_type, import_contacts_request=import_contacts_request)
        print("The response of ListsOtherApi->import_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->import_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **import_contacts_request** | [**ImportContactsRequest**](ImportContactsRequest.md)|  | [optional] 

### Return type

[**ImportContacts**](ImportContacts.md)

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

# **remove_duplicate_contacts**
> RemoveDuplicateContacts remove_duplicate_contacts(list_id, content_type=content_type, remove_duplicate_contacts_request=remove_duplicate_contacts_request)

Remove Duplicate Contacts

_Remove duplicate contacts_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your list id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.remove_duplicate_contacts import RemoveDuplicateContacts
from clicksend.models.remove_duplicate_contacts_request import RemoveDuplicateContactsRequest
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    remove_duplicate_contacts_request = clicksend.RemoveDuplicateContactsRequest() # RemoveDuplicateContactsRequest |  (optional)

    try:
        # Remove Duplicate Contacts
        api_response = api_instance.remove_duplicate_contacts(list_id, content_type=content_type, remove_duplicate_contacts_request=remove_duplicate_contacts_request)
        print("The response of ListsOtherApi->remove_duplicate_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->remove_duplicate_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **remove_duplicate_contacts_request** | [**RemoveDuplicateContactsRequest**](RemoveDuplicateContactsRequest.md)|  | [optional] 

### Return type

[**RemoveDuplicateContacts**](RemoveDuplicateContacts.md)

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

# **remove_opted_out_contacts**
> RemoveOptedOutContacts remove_opted_out_contacts(list_id, opt_out_list_id, content_type=content_type, body=body)

Remove Opted Out Contacts

_Remove all opted out contacts_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your list id |
| opt_out_list_id | path | integer(int32) | true | Your opt out list id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.remove_opted_out_contacts import RemoveOptedOutContacts
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    opt_out_list_id = 'opt_out_list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Remove Opted Out Contacts
        api_response = api_instance.remove_opted_out_contacts(list_id, opt_out_list_id, content_type=content_type, body=body)
        print("The response of ListsOtherApi->remove_opted_out_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->remove_opted_out_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **opt_out_list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**RemoveOptedOutContacts**](RemoveOptedOutContacts.md)

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

# **transfer_contact_to_list**
> TransferContactToList transfer_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)

Transfer Contact to List

_Transfer contact to another list_

Transfer contact to another list

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| from_list_id | path | integer(int32) | true | List ID for list that contains contact. |
| contact_id | path | integer(int32) | true | Contact ID |
| to_list_id | path | integer(int32) | true | List ID for list you want to transfer contact to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.transfer_contact_to_list import TransferContactToList
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
    api_instance = clicksend.ListsOtherApi(api_client)
    from_list_id = 'from_list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    to_list_id = 'to_list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Transfer Contact to List
        api_response = api_instance.transfer_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)
        print("The response of ListsOtherApi->transfer_contact_to_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->transfer_contact_to_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from_list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **to_list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**TransferContactToList**](TransferContactToList.md)

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

# **update_list**
> UpdateList update_list(list_id, content_type=content_type, create_list_request=create_list_request)

Update List

_Update specific contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your list id |
| list_name | body | string | true | Your new list name |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_list_request import CreateListRequest
from clicksend.models.update_list import UpdateList
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_list_request = clicksend.CreateListRequest() # CreateListRequest |  (optional)

    try:
        # Update List
        api_response = api_instance.update_list(list_id, content_type=content_type, create_list_request=create_list_request)
        print("The response of ListsOtherApi->update_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->update_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_list_request** | [**CreateListRequest**](CreateListRequest.md)|  | [optional] 

### Return type

[**UpdateList**](UpdateList.md)

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

# **view_contact_lists**
> view_contact_lists(q=q)

View Contact Lists

_Get list of searched contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| q | query | string | true | Your keyword or query. |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |

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
    api_instance = clicksend.ListsOtherApi(api_client)
    q = 'Test' # str |  (optional)

    try:
        # View Contact Lists
        api_instance.view_contact_lists(q=q)
    except Exception as e:
        print("Exception when calling ListsOtherApi->view_contact_lists: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **str**|  | [optional] 

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

# **view_list_contacts**
> ViewListContacts view_list_contacts(list_id, content_type=content_type)

View List Contacts

_Get all contacts in a list_

### parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Contact list ID |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |
| updated_after | query | integer(int32) | false | Get all contacts updated after a given timestamp. |


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
from clicksend.models.view_list_contacts import ViewListContacts
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View List Contacts
        api_response = api_instance.view_list_contacts(list_id, content_type=content_type)
        print("The response of ListsOtherApi->view_list_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->view_list_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewListContacts**](ViewListContacts.md)

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

# **view_lists**
> ViewLists view_lists(content_type=content_type)

View Lists

_Get all contact lists_

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
from clicksend.models.view_lists import ViewLists
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
    api_instance = clicksend.ListsOtherApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Lists
        api_response = api_instance.view_lists(content_type=content_type)
        print("The response of ListsOtherApi->view_lists:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->view_lists: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewLists**](ViewLists.md)

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

# **view_specific_list**
> ViewSpecificList view_specific_list(list_id, content_type=content_type)

View Specific List

_Get specific contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_list import ViewSpecificList
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
    api_instance = clicksend.ListsOtherApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific List
        api_response = api_instance.view_specific_list(list_id, content_type=content_type)
        print("The response of ListsOtherApi->view_specific_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListsOtherApi->view_specific_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificList**](ViewSpecificList.md)

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

