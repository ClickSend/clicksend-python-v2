# DefaultSenderErrorDetailsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_field** | **str** | The field that caused the error | [optional] 
**reason** | **str** | The error message | [optional] 

## Example

```python
from clicksend.models.default_sender_error_details_inner import DefaultSenderErrorDetailsInner

# TODO update the JSON string below
json = "{}"
# create an instance of DefaultSenderErrorDetailsInner from a JSON string
default_sender_error_details_inner_instance = DefaultSenderErrorDetailsInner.from_json(json)
# print the JSON string representation of the object
print(DefaultSenderErrorDetailsInner.to_json())

# convert the object into a dict
default_sender_error_details_inner_dict = default_sender_error_details_inner_instance.to_dict()
# create an instance of DefaultSenderErrorDetailsInner from a dict
default_sender_error_details_inner_from_dict = DefaultSenderErrorDetailsInner.from_dict(default_sender_error_details_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


