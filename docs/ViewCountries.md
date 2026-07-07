# ViewCountries


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[Country]**](Country.md) |  | [optional] 

## Example

```python
from clicksend.models.view_countries import ViewCountries

# TODO update the JSON string below
json = "{}"
# create an instance of ViewCountries from a JSON string
view_countries_instance = ViewCountries.from_json(json)
# print the JSON string representation of the object
print(ViewCountries.to_json())

# convert the object into a dict
view_countries_dict = view_countries_instance.to_dict()
# create an instance of ViewCountries from a dict
view_countries_from_dict = ViewCountries.from_dict(view_countries_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


