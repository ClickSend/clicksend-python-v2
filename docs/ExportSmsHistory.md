# ExportSmsHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ExportSmsHistoryData**](ExportSmsHistoryData.md) |  | [optional] 

## Example

```python
from clicksend.models.export_sms_history import ExportSmsHistory

# TODO update the JSON string below
json = "{}"
# create an instance of ExportSmsHistory from a JSON string
export_sms_history_instance = ExportSmsHistory.from_json(json)
# print the JSON string representation of the object
print(ExportSmsHistory.to_json())

# convert the object into a dict
export_sms_history_dict = export_sms_history_instance.to_dict()
# create an instance of ExportSmsHistory from a dict
export_sms_history_from_dict = ExportSmsHistory.from_dict(export_sms_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


