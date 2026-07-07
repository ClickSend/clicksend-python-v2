# UpdateDefaultSender


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | HTTP status code of the response. | 
**response_code** | **str** | Code indicating the result of the response. | 
**response_msg** | **str** | Message providing additional information. | 
**data** | [**DefaultSender**](DefaultSender.md) |  | 

## Example

```python
from clicksend.models.update_default_sender import UpdateDefaultSender

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDefaultSender from a JSON string
update_default_sender_instance = UpdateDefaultSender.from_json(json)
# print the JSON string representation of the object
print(UpdateDefaultSender.to_json())

# convert the object into a dict
update_default_sender_dict = update_default_sender_instance.to_dict()
# create an instance of UpdateDefaultSender from a dict
update_default_sender_from_dict = UpdateDefaultSender.from_dict(update_default_sender_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


