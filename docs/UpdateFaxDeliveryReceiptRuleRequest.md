# UpdateFaxDeliveryReceiptRuleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action_address** | **str** |  | [optional] 

## Example

```python
from clicksend.models.update_fax_delivery_receipt_rule_request import UpdateFaxDeliveryReceiptRuleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateFaxDeliveryReceiptRuleRequest from a JSON string
update_fax_delivery_receipt_rule_request_instance = UpdateFaxDeliveryReceiptRuleRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateFaxDeliveryReceiptRuleRequest.to_json())

# convert the object into a dict
update_fax_delivery_receipt_rule_request_dict = update_fax_delivery_receipt_rule_request_instance.to_dict()
# create an instance of UpdateFaxDeliveryReceiptRuleRequest from a dict
update_fax_delivery_receipt_rule_request_from_dict = UpdateFaxDeliveryReceiptRuleRequest.from_dict(update_fax_delivery_receipt_rule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


