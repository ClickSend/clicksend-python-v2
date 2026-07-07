# SmsDeliveryReceiptRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**receipt_rule_id** | **int** | The ID of the receipt rule. | [optional] 
**rule_name** | **str** | The name of the receipt rule. | [optional] 
**match_type** | **int** | The type of match. | [optional] 
**action** | **str** | The type of action. | [optional] 
**action_address** | **str** | The address associated with the action. | [optional] 
**enabled** | **int** | Indicates whether the rule is enabled. | [optional] 

## Example

```python
from clicksend.models.sms_delivery_receipt_rule import SmsDeliveryReceiptRule

# TODO update the JSON string below
json = "{}"
# create an instance of SmsDeliveryReceiptRule from a JSON string
sms_delivery_receipt_rule_instance = SmsDeliveryReceiptRule.from_json(json)
# print the JSON string representation of the object
print(SmsDeliveryReceiptRule.to_json())

# convert the object into a dict
sms_delivery_receipt_rule_dict = sms_delivery_receipt_rule_instance.to_dict()
# create an instance of SmsDeliveryReceiptRule from a dict
sms_delivery_receipt_rule_from_dict = SmsDeliveryReceiptRule.from_dict(sms_delivery_receipt_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


