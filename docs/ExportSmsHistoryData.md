# ExportSmsHistoryData

The parameters related to the generated SMS history file.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | The download link to the generated SMS history file. | [optional] 

## Example

```python
from clicksend.models.export_sms_history_data import ExportSmsHistoryData

# TODO update the JSON string below
json = "{}"
# create an instance of ExportSmsHistoryData from a JSON string
export_sms_history_data_instance = ExportSmsHistoryData.from_json(json)
# print the JSON string representation of the object
print(ExportSmsHistoryData.to_json())

# convert the object into a dict
export_sms_history_data_dict = export_sms_history_data_instance.to_dict()
# create an instance of ExportSmsHistoryData from a dict
export_sms_history_data_from_dict = ExportSmsHistoryData.from_dict(export_sms_history_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


