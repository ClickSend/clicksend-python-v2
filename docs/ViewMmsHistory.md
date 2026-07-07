# ViewMmsHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewMmsHistoryData**](ViewMmsHistoryData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_mms_history import ViewMmsHistory

# TODO update the JSON string below
json = "{}"
# create an instance of ViewMmsHistory from a JSON string
view_mms_history_instance = ViewMmsHistory.from_json(json)
# print the JSON string representation of the object
print(ViewMmsHistory.to_json())

# convert the object into a dict
view_mms_history_dict = view_mms_history_instance.to_dict()
# create an instance of ViewMmsHistory from a dict
view_mms_history_from_dict = ViewMmsHistory.from_dict(view_mms_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


