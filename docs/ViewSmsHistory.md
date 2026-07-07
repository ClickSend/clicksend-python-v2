# ViewSmsHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewSmsHistoryData**](ViewSmsHistoryData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_history import ViewSmsHistory

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsHistory from a JSON string
view_sms_history_instance = ViewSmsHistory.from_json(json)
# print the JSON string representation of the object
print(ViewSmsHistory.to_json())

# convert the object into a dict
view_sms_history_dict = view_sms_history_instance.to_dict()
# create an instance of ViewSmsHistory from a dict
view_sms_history_from_dict = ViewSmsHistory.from_dict(view_sms_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


