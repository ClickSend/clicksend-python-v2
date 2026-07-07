# clicksend.InternationalMessagingApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**agree_to_rules_and_regulation**](InternationalMessagingApi.md#agree_to_rules_and_regulation) | **POST** /v3/user-countries/agree | Agree to rules and regulation
[**get_countries_for_global_sending**](InternationalMessagingApi.md#get_countries_for_global_sending) | **GET** /v3/user-countries | Get Countries for Global Sending
[**list_countries**](InternationalMessagingApi.md#list_countries) | **GET** /v3/country-list | International Messaging
[**select_countries_for_global_sending**](InternationalMessagingApi.md#select_countries_for_global_sending) | **POST** /v3/user-countries | Select Countries for Global Sending
[**timezones**](InternationalMessagingApi.md#timezones) | **GET** /v3/timezones | Timezones
[**view_countries**](InternationalMessagingApi.md#view_countries) | **GET** /v3/countries | View Countries


# **agree_to_rules_and_regulation**
> AgreeToRulesAndRegulation agree_to_rules_and_regulation()

Agree to rules and regulation

_Update Country Rule_

To agree on rules and regulations of selected countries and confirm selection.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| country_list_ids | number | true | none | Country list ID's |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.agree_to_rules_and_regulation import AgreeToRulesAndRegulation
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
    api_instance = clicksend.InternationalMessagingApi(api_client)

    try:
        # Agree to rules and regulation
        api_response = api_instance.agree_to_rules_and_regulation()
        print("The response of InternationalMessagingApi->agree_to_rules_and_regulation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternationalMessagingApi->agree_to_rules_and_regulation: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AgreeToRulesAndRegulation**](AgreeToRulesAndRegulation.md)

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

# **get_countries_for_global_sending**
> GetCountriesForGlobalSending get_countries_for_global_sending()

Get Countries for Global Sending

_Get Countries for global sending_

Get the list of selected countries.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_countries_for_global_sending import GetCountriesForGlobalSending
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
    api_instance = clicksend.InternationalMessagingApi(api_client)

    try:
        # Get Countries for Global Sending
        api_response = api_instance.get_countries_for_global_sending()
        print("The response of InternationalMessagingApi->get_countries_for_global_sending:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternationalMessagingApi->get_countries_for_global_sending: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**GetCountriesForGlobalSending**](GetCountriesForGlobalSending.md)

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

# **list_countries**
> ListCountries list_countries()

International Messaging

_List of countries_

List of countries with IDs that can be used in selecting countries for Global sending.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_countries import ListCountries
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
    api_instance = clicksend.InternationalMessagingApi(api_client)

    try:
        # International Messaging
        api_response = api_instance.list_countries()
        print("The response of InternationalMessagingApi->list_countries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternationalMessagingApi->list_countries: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ListCountries**](ListCountries.md)

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

# **select_countries_for_global_sending**
> SelectCountriesForGlobalSending select_countries_for_global_sending(select_countries_for_global_sending_request=select_countries_for_global_sending_request)

Select Countries for Global Sending

_Select Countries_

Use this endpoint to select countries that you intend to send sms / mms to. To remove / unselect a country, just remove the country id from the array in the payload.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| country_list_ids | number | true | none | Country list ID's |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.select_countries_for_global_sending import SelectCountriesForGlobalSending
from clicksend.models.select_countries_for_global_sending_request import SelectCountriesForGlobalSendingRequest
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
    api_instance = clicksend.InternationalMessagingApi(api_client)
    select_countries_for_global_sending_request = clicksend.SelectCountriesForGlobalSendingRequest() # SelectCountriesForGlobalSendingRequest |  (optional)

    try:
        # Select Countries for Global Sending
        api_response = api_instance.select_countries_for_global_sending(select_countries_for_global_sending_request=select_countries_for_global_sending_request)
        print("The response of InternationalMessagingApi->select_countries_for_global_sending:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternationalMessagingApi->select_countries_for_global_sending: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_countries_for_global_sending_request** | [**SelectCountriesForGlobalSendingRequest**](SelectCountriesForGlobalSendingRequest.md)|  | [optional] 

### Return type

[**SelectCountriesForGlobalSending**](SelectCountriesForGlobalSending.md)

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

# **timezones**
> Timezones timezones(content_type=content_type)

Timezones

_Get supported list of timezones._

Get supported list of timezones.

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
from clicksend.models.timezones import Timezones
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
    api_instance = clicksend.InternationalMessagingApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Timezones
        api_response = api_instance.timezones(content_type=content_type)
        print("The response of InternationalMessagingApi->timezones:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternationalMessagingApi->timezones: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**Timezones**](Timezones.md)

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

# **view_countries**
> ViewCountries view_countries()

View Countries

_Get all country codes_

Get all countries


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #6BBD5B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint does not require authentication</span> 
</div>

### Example


```python
import clicksend
from clicksend.models.view_countries import ViewCountries
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)


# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.InternationalMessagingApi(api_client)

    try:
        # View Countries
        api_response = api_instance.view_countries()
        print("The response of InternationalMessagingApi->view_countries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternationalMessagingApi->view_countries: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ViewCountries**](ViewCountries.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

