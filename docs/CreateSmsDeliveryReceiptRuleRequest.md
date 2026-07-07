# CreateSmsDeliveryReceiptRuleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule_name** | **str** |  | [optional] 
**match_type** | **int** |  | [optional] 
**action** | **str** |  | [optional] 
**action_address** | **str** |  | [optional] 
**enabled** | **int** |  | [optional] 

## Example

```python
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSmsDeliveryReceiptRuleRequest from a JSON string
create_sms_delivery_receipt_rule_request_instance = CreateSmsDeliveryReceiptRuleRequest.from_json(json)
# print the JSON string representation of the object
print(CreateSmsDeliveryReceiptRuleRequest.to_json())

# convert the object into a dict
create_sms_delivery_receipt_rule_request_dict = create_sms_delivery_receipt_rule_request_instance.to_dict()
# create an instance of CreateSmsDeliveryReceiptRuleRequest from a dict
create_sms_delivery_receipt_rule_request_from_dict = CreateSmsDeliveryReceiptRuleRequest.from_dict(create_sms_delivery_receipt_rule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


