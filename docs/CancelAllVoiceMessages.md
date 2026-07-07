# CancelAllVoiceMessages


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.cancel_all_voice_messages import CancelAllVoiceMessages

# TODO update the JSON string below
json = "{}"
# create an instance of CancelAllVoiceMessages from a JSON string
cancel_all_voice_messages_instance = CancelAllVoiceMessages.from_json(json)
# print the JSON string representation of the object
print(CancelAllVoiceMessages.to_json())

# convert the object into a dict
cancel_all_voice_messages_dict = cancel_all_voice_messages_instance.to_dict()
# create an instance of CancelAllVoiceMessages from a dict
cancel_all_voice_messages_from_dict = CancelAllVoiceMessages.from_dict(cancel_all_voice_messages_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


