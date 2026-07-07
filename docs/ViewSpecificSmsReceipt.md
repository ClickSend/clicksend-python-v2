# ViewSpecificSmsReceipt


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information.  This parameter doesn’t reflect the status of each message. Check the _status_ parameter of the message object to view the status of the individual message. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SmsReceipt**](SmsReceipt.md) |  | [optional] 

## Example

```python
from clicksend.models.view_specific_sms_receipt import ViewSpecificSmsReceipt

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSpecificSmsReceipt from a JSON string
view_specific_sms_receipt_instance = ViewSpecificSmsReceipt.from_json(json)
# print the JSON string representation of the object
print(ViewSpecificSmsReceipt.to_json())

# convert the object into a dict
view_specific_sms_receipt_dict = view_specific_sms_receipt_instance.to_dict()
# create an instance of ViewSpecificSmsReceipt from a dict
view_specific_sms_receipt_from_dict = ViewSpecificSmsReceipt.from_dict(view_specific_sms_receipt_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


