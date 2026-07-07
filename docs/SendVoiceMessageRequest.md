# SendVoiceMessageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**messages** | [**List[SendVoiceMessageRequestMessagesInner]**](SendVoiceMessageRequestMessagesInner.md) |  | [optional] 

## Example

```python
from clicksend.models.send_voice_message_request import SendVoiceMessageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendVoiceMessageRequest from a JSON string
send_voice_message_request_instance = SendVoiceMessageRequest.from_json(json)
# print the JSON string representation of the object
print(SendVoiceMessageRequest.to_json())

# convert the object into a dict
send_voice_message_request_dict = send_voice_message_request_instance.to_dict()
# create an instance of SendVoiceMessageRequest from a dict
send_voice_message_request_from_dict = SendVoiceMessageRequest.from_dict(send_voice_message_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


