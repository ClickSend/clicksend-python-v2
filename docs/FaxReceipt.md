# FaxReceipt


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp_send** | **str** | The timestamp when the message was sent. | [optional] 
**timestamp** | **str** | The timestamp associated with the message. | [optional] 
**message_id** | **str** | The ID of the message. | [optional] 
**status_code** | **str** | The status code of the message. | [optional] 
**status_text** | **str** | The status text of the message. | [optional] 
**error_code** | **str** | The error code associated with the message. | [optional] 
**error_text** | **str** | The error text associated with the message. | [optional] 
**custom_string** | **str** | A custom string associated with the message. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount. | [optional] 
**message_type** | **str** | The type of message. | [optional] 

## Example

```python
from clicksend.models.fax_receipt import FaxReceipt

# TODO update the JSON string below
json = "{}"
# create an instance of FaxReceipt from a JSON string
fax_receipt_instance = FaxReceipt.from_json(json)
# print the JSON string representation of the object
print(FaxReceipt.to_json())

# convert the object into a dict
fax_receipt_dict = fax_receipt_instance.to_dict()
# create an instance of FaxReceipt from a dict
fax_receipt_from_dict = FaxReceipt.from_dict(fax_receipt_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


