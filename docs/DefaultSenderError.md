# DefaultSenderError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | HTTP status code of the response. | 
**response_code** | **str** | Code indicating the result of the response. | 
**response_msg** | **str** | Message providing additional information. | 
**data** | **object** |  | [optional] 
**details** | [**List[DefaultSenderErrorDetailsInner]**](DefaultSenderErrorDetailsInner.md) | List of error details | 

## Example

```python
from clicksend.models.default_sender_error import DefaultSenderError

# TODO update the JSON string below
json = "{}"
# create an instance of DefaultSenderError from a JSON string
default_sender_error_instance = DefaultSenderError.from_json(json)
# print the JSON string representation of the object
print(DefaultSenderError.to_json())

# convert the object into a dict
default_sender_error_dict = default_sender_error_instance.to_dict()
# create an instance of DefaultSenderError from a dict
default_sender_error_from_dict = DefaultSenderError.from_dict(default_sender_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


