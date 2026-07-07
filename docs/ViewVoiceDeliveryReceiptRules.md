# ViewVoiceDeliveryReceiptRules


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewVoiceDeliveryReceiptRulesData**](ViewVoiceDeliveryReceiptRulesData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_voice_delivery_receipt_rules import ViewVoiceDeliveryReceiptRules

# TODO update the JSON string below
json = "{}"
# create an instance of ViewVoiceDeliveryReceiptRules from a JSON string
view_voice_delivery_receipt_rules_instance = ViewVoiceDeliveryReceiptRules.from_json(json)
# print the JSON string representation of the object
print(ViewVoiceDeliveryReceiptRules.to_json())

# convert the object into a dict
view_voice_delivery_receipt_rules_dict = view_voice_delivery_receipt_rules_instance.to_dict()
# create an instance of ViewVoiceDeliveryReceiptRules from a dict
view_voice_delivery_receipt_rules_from_dict = ViewVoiceDeliveryReceiptRules.from_dict(view_voice_delivery_receipt_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


