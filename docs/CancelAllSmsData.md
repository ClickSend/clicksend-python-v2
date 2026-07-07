# CancelAllSmsData

The parameters related to the cancelled scheduled SMS.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **int** | The number of scehduled SMS cancelled. | [optional] 

## Example

```python
from clicksend.models.cancel_all_sms_data import CancelAllSmsData

# TODO update the JSON string below
json = "{}"
# create an instance of CancelAllSmsData from a JSON string
cancel_all_sms_data_instance = CancelAllSmsData.from_json(json)
# print the JSON string representation of the object
print(CancelAllSmsData.to_json())

# convert the object into a dict
cancel_all_sms_data_dict = cancel_all_sms_data_instance.to_dict()
# create an instance of CancelAllSmsData from a dict
cancel_all_sms_data_from_dict = CancelAllSmsData.from_dict(cancel_all_sms_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


