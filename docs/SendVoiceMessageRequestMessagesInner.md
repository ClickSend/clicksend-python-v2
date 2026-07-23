# SendVoiceMessageRequestMessagesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**to** | **str** |  | [optional] 
**voice** | **str** |  | [optional] 
**lang** | **str** |  | [optional] 
**machine_detection** | **int** |  | [optional] 

## Example

```python
from clicksend.models.send_voice_message_request_messages_inner import SendVoiceMessageRequestMessagesInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendVoiceMessageRequestMessagesInner from a JSON string
send_voice_message_request_messages_inner_instance = SendVoiceMessageRequestMessagesInner.from_json(json)
# print the JSON string representation of the object
print(SendVoiceMessageRequestMessagesInner.to_json())

# convert the object into a dict
send_voice_message_request_messages_inner_dict = send_voice_message_request_messages_inner_instance.to_dict()
# create an instance of SendVoiceMessageRequestMessagesInner from a dict
send_voice_message_request_messages_inner_from_dict = SendVoiceMessageRequestMessagesInner.from_dict(send_voice_message_request_messages_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


