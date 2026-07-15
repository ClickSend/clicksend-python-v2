# VoiceMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **str** | The date, if applicable. May be null; see also &#x60;date_added&#x60;. | [optional] 
**date_added** | **int** | The Unix timestamp when the message was added. | [optional] 
**list_id** | **str** | The ID of the list associated with the message, if applicable. | [optional] 
**to** | **str** | The recipient&#39;s phone number. | [optional] 
**to_type** | **str** | The type of recipient. | [optional] 
**body** | **str** | The body of the message. | [optional] 
**var_from** | **str** | The sender&#39;s phone number. | [optional] 
**lang** | **str** | The language of the message. | [optional] 
**voice** | **str** | The voice of the message. | [optional] 
**schedule** | [**VoiceMessageSchedule**](VoiceMessageSchedule.md) |  | [optional] 
**message_id** | **str** | The ID of the message. | [optional] 
**message_parts** | [**VoiceMessageSchedule**](VoiceMessageSchedule.md) |  | [optional] 
**message_price** | **str** | The price of the message. | [optional] 
**custom_string** | **str** | The custom string of the message. | [optional] 
**user_id** | **float** | The ID of the user. | [optional] 
**subaccount_id** | **float** | The ID of the subaccount. | [optional] 
**country** | **str** | The country code of the message. | [optional] 
**require_input** | **float** | The require input of the message. | [optional] 
**machine_detection** | **float** | The machine detection of the message. | [optional] 
**machine_detected** | **float** | Flag indicating if an answering machine was detected. | [optional] 
**digits** | **str** | The digits entered by the recipient, if any input was collected. | [optional] 
**carrier** | **str** | The carrier of the recipient&#39;s phone number. | [optional] 
**status_code** | **str** | The status code of the message. | [optional] 
**status_text** | **str** | A human-readable description of the status. | [optional] 
**status** | **str** | The status of the message. | [optional] 
**api_username** | **str** | The API username associated with the message. | [optional] 

## Example

```python
from clicksend.models.voice_message import VoiceMessage

# TODO update the JSON string below
json = "{}"
# create an instance of VoiceMessage from a JSON string
voice_message_instance = VoiceMessage.from_json(json)
# print the JSON string representation of the object
print(VoiceMessage.to_json())

# convert the object into a dict
voice_message_dict = voice_message_instance.to_dict()
# create an instance of VoiceMessage from a dict
voice_message_from_dict = VoiceMessage.from_dict(voice_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


