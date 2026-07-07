# CancelAllSms


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.cancel_all_sms import CancelAllSms

# TODO update the JSON string below
json = "{}"
# create an instance of CancelAllSms from a JSON string
cancel_all_sms_instance = CancelAllSms.from_json(json)
# print the JSON string representation of the object
print(CancelAllSms.to_json())

# convert the object into a dict
cancel_all_sms_dict = cancel_all_sms_instance.to_dict()
# create an instance of CancelAllSms from a dict
cancel_all_sms_from_dict = CancelAllSms.from_dict(cancel_all_sms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


