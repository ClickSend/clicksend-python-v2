# ListCountries


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[ListCountriesDataInner]**](ListCountriesDataInner.md) |  | [optional] 

## Example

```python
from clicksend.models.list_countries import ListCountries

# TODO update the JSON string below
json = "{}"
# create an instance of ListCountries from a JSON string
list_countries_instance = ListCountries.from_json(json)
# print the JSON string representation of the object
print(ListCountries.to_json())

# convert the object into a dict
list_countries_dict = list_countries_instance.to_dict()
# create an instance of ListCountries from a dict
list_countries_from_dict = ListCountries.from_dict(list_countries_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


