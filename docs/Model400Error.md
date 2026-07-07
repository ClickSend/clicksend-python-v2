# Model400Error


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | HTTP status code of the response. | 
**response_code** | **str** | Code indicating the result of the response. | 
**response_msg** | **str** | Message providing additional information. | 
**data** | **object** |  | [optional] 

## Example

```python
from clicksend.models.model400_error import Model400Error

# TODO update the JSON string below
json = "{}"
# create an instance of Model400Error from a JSON string
model400_error_instance = Model400Error.from_json(json)
# print the JSON string representation of the object
print(Model400Error.to_json())

# convert the object into a dict
model400_error_dict = model400_error_instance.to_dict()
# create an instance of Model400Error from a dict
model400_error_from_dict = Model400Error.from_dict(model400_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


