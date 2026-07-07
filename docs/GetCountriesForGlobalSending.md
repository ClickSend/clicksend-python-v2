# GetCountriesForGlobalSending


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[GlobalSending]**](GlobalSending.md) |  | [optional] 

## Example

```python
from clicksend.models.get_countries_for_global_sending import GetCountriesForGlobalSending

# TODO update the JSON string below
json = "{}"
# create an instance of GetCountriesForGlobalSending from a JSON string
get_countries_for_global_sending_instance = GetCountriesForGlobalSending.from_json(json)
# print the JSON string representation of the object
print(GetCountriesForGlobalSending.to_json())

# convert the object into a dict
get_countries_for_global_sending_dict = get_countries_for_global_sending_instance.to_dict()
# create an instance of GetCountriesForGlobalSending from a dict
get_countries_for_global_sending_from_dict = GetCountriesForGlobalSending.from_dict(get_countries_for_global_sending_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


