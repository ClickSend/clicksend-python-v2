# EmailDeliveryReceiptRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**receipt_rule_id** | **int** | The ID of the receipt rule. | [optional] 
**rule_name** | **str** | The name of the receipt rule. | [optional] 
**match_type** | **int** | The type of match for the rule. | [optional] 
**action** | **str** | The action to be taken by the rule. | [optional] 
**action_address** | **str** | The address associated with the action. | [optional] 
**enabled** | **int** | Indicates whether the rule is enabled. | [optional] 

## Example

```python
from clicksend.models.email_delivery_receipt_rule import EmailDeliveryReceiptRule

# TODO update the JSON string below
json = "{}"
# create an instance of EmailDeliveryReceiptRule from a JSON string
email_delivery_receipt_rule_instance = EmailDeliveryReceiptRule.from_json(json)
# print the JSON string representation of the object
print(EmailDeliveryReceiptRule.to_json())

# convert the object into a dict
email_delivery_receipt_rule_dict = email_delivery_receipt_rule_instance.to_dict()
# create an instance of EmailDeliveryReceiptRule from a dict
email_delivery_receipt_rule_from_dict = EmailDeliveryReceiptRule.from_dict(email_delivery_receipt_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


