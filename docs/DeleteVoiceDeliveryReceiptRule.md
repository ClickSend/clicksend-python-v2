# DeleteVoiceDeliveryReceiptRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **List[str]** |  | [optional] 

## Example

```python
from clicksend.models.delete_voice_delivery_receipt_rule import DeleteVoiceDeliveryReceiptRule

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteVoiceDeliveryReceiptRule from a JSON string
delete_voice_delivery_receipt_rule_instance = DeleteVoiceDeliveryReceiptRule.from_json(json)
# print the JSON string representation of the object
print(DeleteVoiceDeliveryReceiptRule.to_json())

# convert the object into a dict
delete_voice_delivery_receipt_rule_dict = delete_voice_delivery_receipt_rule_instance.to_dict()
# create an instance of DeleteVoiceDeliveryReceiptRule from a dict
delete_voice_delivery_receipt_rule_from_dict = DeleteVoiceDeliveryReceiptRule.from_dict(delete_voice_delivery_receipt_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


