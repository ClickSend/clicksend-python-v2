# UpdateDefaultSenderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**default_sender_strategies** | [**List[CreateDefaultSenderRequestDefaultSenderStrategiesInner]**](CreateDefaultSenderRequestDefaultSenderStrategiesInner.md) | Array detailing sender strategies. Must contain exactly 1 element. Multiple strategies support coming soon. | 

## Example

```python
from clicksend.models.update_default_sender_request import UpdateDefaultSenderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDefaultSenderRequest from a JSON string
update_default_sender_request_instance = UpdateDefaultSenderRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateDefaultSenderRequest.to_json())

# convert the object into a dict
update_default_sender_request_dict = update_default_sender_request_instance.to_dict()
# create an instance of UpdateDefaultSenderRequest from a dict
update_default_sender_request_from_dict = UpdateDefaultSenderRequest.from_dict(update_default_sender_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


