# CreateDefaultSender


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | HTTP status code of the response. | 
**response_code** | **str** | Code indicating the result of the response. | 
**response_msg** | **str** | Message providing additional information. | 
**data** | [**DefaultSender**](DefaultSender.md) |  | 

## Example

```python
from clicksend.models.create_default_sender import CreateDefaultSender

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDefaultSender from a JSON string
create_default_sender_instance = CreateDefaultSender.from_json(json)
# print the JSON string representation of the object
print(CreateDefaultSender.to_json())

# convert the object into a dict
create_default_sender_dict = create_default_sender_instance.to_dict()
# create an instance of CreateDefaultSender from a dict
create_default_sender_from_dict = CreateDefaultSender.from_dict(create_default_sender_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


