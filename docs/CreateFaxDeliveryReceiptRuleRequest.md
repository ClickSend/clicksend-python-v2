# CreateFaxDeliveryReceiptRuleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule_name** | **str** |  | [optional] 
**match_type** | **int** |  | [optional] 
**action** | **str** |  | [optional] 
**action_address** | **str** |  | [optional] 
**enabled** | **int** |  | [optional] 
**url** | **str** |  | [optional] 

## Example

```python
from clicksend.models.create_fax_delivery_receipt_rule_request import CreateFaxDeliveryReceiptRuleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateFaxDeliveryReceiptRuleRequest from a JSON string
create_fax_delivery_receipt_rule_request_instance = CreateFaxDeliveryReceiptRuleRequest.from_json(json)
# print the JSON string representation of the object
print(CreateFaxDeliveryReceiptRuleRequest.to_json())

# convert the object into a dict
create_fax_delivery_receipt_rule_request_dict = create_fax_delivery_receipt_rule_request_instance.to_dict()
# create an instance of CreateFaxDeliveryReceiptRuleRequest from a dict
create_fax_delivery_receipt_rule_request_from_dict = CreateFaxDeliveryReceiptRuleRequest.from_dict(create_fax_delivery_receipt_rule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


