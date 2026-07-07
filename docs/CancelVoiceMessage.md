# CancelVoiceMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **List[str]** |  | [optional] 

## Example

```python
from clicksend.models.cancel_voice_message import CancelVoiceMessage

# TODO update the JSON string below
json = "{}"
# create an instance of CancelVoiceMessage from a JSON string
cancel_voice_message_instance = CancelVoiceMessage.from_json(json)
# print the JSON string representation of the object
print(CancelVoiceMessage.to_json())

# convert the object into a dict
cancel_voice_message_dict = cancel_voice_message_instance.to_dict()
# create an instance of CancelVoiceMessage from a dict
cancel_voice_message_from_dict = CancelVoiceMessage.from_dict(cancel_voice_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


