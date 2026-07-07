# ViewSmsReceipts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information.  This parameter doesn’t reflect the status of each message. Check the _status_ parameter of the message object to view the status of the individual message. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewSmsReceiptsData**](ViewSmsReceiptsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_receipts import ViewSmsReceipts

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsReceipts from a JSON string
view_sms_receipts_instance = ViewSmsReceipts.from_json(json)
# print the JSON string representation of the object
print(ViewSmsReceipts.to_json())

# convert the object into a dict
view_sms_receipts_dict = view_sms_receipts_instance.to_dict()
# create an instance of ViewSmsReceipts from a dict
view_sms_receipts_from_dict = ViewSmsReceipts.from_dict(view_sms_receipts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


