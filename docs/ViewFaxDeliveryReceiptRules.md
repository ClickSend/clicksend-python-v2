# ViewFaxDeliveryReceiptRules


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewFaxDeliveryReceiptRulesData**](ViewFaxDeliveryReceiptRulesData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_fax_delivery_receipt_rules import ViewFaxDeliveryReceiptRules

# TODO update the JSON string below
json = "{}"
# create an instance of ViewFaxDeliveryReceiptRules from a JSON string
view_fax_delivery_receipt_rules_instance = ViewFaxDeliveryReceiptRules.from_json(json)
# print the JSON string representation of the object
print(ViewFaxDeliveryReceiptRules.to_json())

# convert the object into a dict
view_fax_delivery_receipt_rules_dict = view_fax_delivery_receipt_rules_instance.to_dict()
# create an instance of ViewFaxDeliveryReceiptRules from a dict
view_fax_delivery_receipt_rules_from_dict = ViewFaxDeliveryReceiptRules.from_dict(view_fax_delivery_receipt_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


