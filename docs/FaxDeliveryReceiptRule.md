# FaxDeliveryReceiptRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**receipt_rule_id** | **int** | The ID of the receipt rule. | [optional] 
**rule_name** | **str** | The name of the receipt rule. | [optional] 
**match_type** | **int** | The type of match. | [optional] 
**action** | **str** | The action triggered by the rule. | [optional] 
**action_address** | **str** | The address associated with the action. | [optional] 
**enabled** | **int** | Indicates whether the rule is enabled. | [optional] 

## Example

```python
from clicksend.models.fax_delivery_receipt_rule import FaxDeliveryReceiptRule

# TODO update the JSON string below
json = "{}"
# create an instance of FaxDeliveryReceiptRule from a JSON string
fax_delivery_receipt_rule_instance = FaxDeliveryReceiptRule.from_json(json)
# print the JSON string representation of the object
print(FaxDeliveryReceiptRule.to_json())

# convert the object into a dict
fax_delivery_receipt_rule_dict = fax_delivery_receipt_rule_instance.to_dict()
# create an instance of FaxDeliveryReceiptRule from a dict
fax_delivery_receipt_rule_from_dict = FaxDeliveryReceiptRule.from_dict(fax_delivery_receipt_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


