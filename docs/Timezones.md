# Timezones


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **List[str]** |  | [optional] 

## Example

```python
from clicksend.models.timezones import Timezones

# TODO update the JSON string below
json = "{}"
# create an instance of Timezones from a JSON string
timezones_instance = Timezones.from_json(json)
# print the JSON string representation of the object
print(Timezones.to_json())

# convert the object into a dict
timezones_dict = timezones_instance.to_dict()
# create an instance of Timezones from a dict
timezones_from_dict = Timezones.from_dict(timezones_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


