# ListCountriesDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The id of the country. | [optional] 
**name** | **str** | The name of the country. | [optional] 
**code** | **str** | The code of the country. | [optional] 
**region** | **str** | The region of the country. | [optional] 

## Example

```python
from clicksend.models.list_countries_data_inner import ListCountriesDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCountriesDataInner from a JSON string
list_countries_data_inner_instance = ListCountriesDataInner.from_json(json)
# print the JSON string representation of the object
print(ListCountriesDataInner.to_json())

# convert the object into a dict
list_countries_data_inner_dict = list_countries_data_inner_instance.to_dict()
# create an instance of ListCountriesDataInner from a dict
list_countries_data_inner_from_dict = ListCountriesDataInner.from_dict(list_countries_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


