# VoiceMessageSchedule

The timestamp when the message should be sent, as a <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix timestamp</a>. Returned as an empty string when no schedule was set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------

## Example

```python
from clicksend.models.voice_message_schedule import VoiceMessageSchedule

# TODO update the JSON string below
json = "{}"
# create an instance of VoiceMessageSchedule from a JSON string
voice_message_schedule_instance = VoiceMessageSchedule.from_json(json)
# print the JSON string representation of the object
print(VoiceMessageSchedule.to_json())

# convert the object into a dict
voice_message_schedule_dict = voice_message_schedule_instance.to_dict()
# create an instance of VoiceMessageSchedule from a dict
voice_message_schedule_from_dict = VoiceMessageSchedule.from_dict(voice_message_schedule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


