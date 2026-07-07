# SendVoiceMessageData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_price** | **float** | The total price of the message. | [optional] 
**total_count** | **float** | The total count of the message. | [optional] 
**queued_count** | **float** | The count of the queued message. | [optional] 
**messages** | [**List[VoiceMessage]**](VoiceMessage.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.send_voice_message_data import SendVoiceMessageData

# TODO update the JSON string below
json = "{}"
# create an instance of SendVoiceMessageData from a JSON string
send_voice_message_data_instance = SendVoiceMessageData.from_json(json)
# print the JSON string representation of the object
print(SendVoiceMessageData.to_json())

# convert the object into a dict
send_voice_message_data_dict = send_voice_message_data_instance.to_dict()
# create an instance of SendVoiceMessageData from a dict
send_voice_message_data_from_dict = SendVoiceMessageData.from_dict(send_voice_message_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


