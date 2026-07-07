# ExportVoiceHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ExportSmsHistoryData**](ExportSmsHistoryData.md) |  | [optional] 

## Example

```python
from clicksend.models.export_voice_history import ExportVoiceHistory

# TODO update the JSON string below
json = "{}"
# create an instance of ExportVoiceHistory from a JSON string
export_voice_history_instance = ExportVoiceHistory.from_json(json)
# print the JSON string representation of the object
print(ExportVoiceHistory.to_json())

# convert the object into a dict
export_voice_history_dict = export_voice_history_instance.to_dict()
# create an instance of ExportVoiceHistory from a dict
export_voice_history_from_dict = ExportVoiceHistory.from_dict(export_voice_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


