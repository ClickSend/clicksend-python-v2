# GetVoiceHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**GetVoiceHistoryData**](GetVoiceHistoryData.md) |  | [optional] 

## Example

```python
from clicksend.models.get_voice_history import GetVoiceHistory

# TODO update the JSON string below
json = "{}"
# create an instance of GetVoiceHistory from a JSON string
get_voice_history_instance = GetVoiceHistory.from_json(json)
# print the JSON string representation of the object
print(GetVoiceHistory.to_json())

# convert the object into a dict
get_voice_history_dict = get_voice_history_instance.to_dict()
# create an instance of GetVoiceHistory from a dict
get_voice_history_from_dict = GetVoiceHistory.from_dict(get_voice_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


