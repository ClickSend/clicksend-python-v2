# ViewFaxHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewFaxHistoryData**](ViewFaxHistoryData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_fax_history import ViewFaxHistory

# TODO update the JSON string below
json = "{}"
# create an instance of ViewFaxHistory from a JSON string
view_fax_history_instance = ViewFaxHistory.from_json(json)
# print the JSON string representation of the object
print(ViewFaxHistory.to_json())

# convert the object into a dict
view_fax_history_dict = view_fax_history_instance.to_dict()
# create an instance of ViewFaxHistory from a dict
view_fax_history_from_dict = ViewFaxHistory.from_dict(view_fax_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


