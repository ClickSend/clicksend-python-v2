# SendVoiceMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | Here are your data. | [optional] 
**data** | [**SendVoiceMessageData**](SendVoiceMessageData.md) |  | [optional] 

## Example

```python
from clicksend.models.send_voice_message import SendVoiceMessage

# TODO update the JSON string below
json = "{}"
# create an instance of SendVoiceMessage from a JSON string
send_voice_message_instance = SendVoiceMessage.from_json(json)
# print the JSON string representation of the object
print(SendVoiceMessage.to_json())

# convert the object into a dict
send_voice_message_dict = send_voice_message_instance.to_dict()
# create an instance of SendVoiceMessage from a dict
send_voice_message_from_dict = SendVoiceMessage.from_dict(send_voice_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


