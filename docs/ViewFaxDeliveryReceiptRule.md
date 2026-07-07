# ViewFaxDeliveryReceiptRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**FaxDeliveryReceiptRule**](FaxDeliveryReceiptRule.md) |  | [optional] 

## Example

```python
from clicksend.models.view_fax_delivery_receipt_rule import ViewFaxDeliveryReceiptRule

# TODO update the JSON string below
json = "{}"
# create an instance of ViewFaxDeliveryReceiptRule from a JSON string
view_fax_delivery_receipt_rule_instance = ViewFaxDeliveryReceiptRule.from_json(json)
# print the JSON string representation of the object
print(ViewFaxDeliveryReceiptRule.to_json())

# convert the object into a dict
view_fax_delivery_receipt_rule_dict = view_fax_delivery_receipt_rule_instance.to_dict()
# create an instance of ViewFaxDeliveryReceiptRule from a dict
view_fax_delivery_receipt_rule_from_dict = ViewFaxDeliveryReceiptRule.from_dict(view_fax_delivery_receipt_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


