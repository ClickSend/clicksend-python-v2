# VoiceReceipt


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp_send** | **str** | Timestamp of the original send request in UNIX format. e.g 1439173980 | [optional] 
**timestamp** | **str** | Timestamp of delivery report in UNIX format. e.g 1439173981 | [optional] 
**message_id** | **str** | Message ID, returned when originally sending the message. | [optional] 
**status_code** | **str** | Status code. Refer to &#39;Voice Delivery Status Codes&#39; in docs. | [optional] 
**status_text** | **str** | Status text. | [optional] 
**error_code** | **str** | Error code. | [optional] 
**error_text** | **str** | Error text. | [optional] 
**custom_string** | **str** | A custom string used when sending the original message. | [optional] 
**message_type** | **str** | voice (constant). | [optional] 
**digits** | **str** | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn&#39;t provide any input. | [optional] 

## Example

```python
from clicksend.models.voice_receipt import VoiceReceipt

# TODO update the JSON string below
json = "{}"
# create an instance of VoiceReceipt from a JSON string
voice_receipt_instance = VoiceReceipt.from_json(json)
# print the JSON string representation of the object
print(VoiceReceipt.to_json())

# convert the object into a dict
voice_receipt_dict = voice_receipt_instance.to_dict()
# create an instance of VoiceReceipt from a dict
voice_receipt_from_dict = VoiceReceipt.from_dict(voice_receipt_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


