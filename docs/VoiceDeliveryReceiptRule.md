# VoiceDeliveryReceiptRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**receipt_rule_id** | **int** | The ID of the receipt rule. | [optional] 
**rule_name** | **str** | The name of the receipt rule. | [optional] 
**match_type** | **int** | The match type of the receipt rule. | [optional] 
**action** | **str** | The action of the receipt rule. | [optional] 
**action_address** | **str** | The action address of the receipt rule. | [optional] 
**enabled** | **int** | The enabled status of the receipt rule. | [optional] 

## Example

```python
from clicksend.models.voice_delivery_receipt_rule import VoiceDeliveryReceiptRule

# TODO update the JSON string below
json = "{}"
# create an instance of VoiceDeliveryReceiptRule from a JSON string
voice_delivery_receipt_rule_instance = VoiceDeliveryReceiptRule.from_json(json)
# print the JSON string representation of the object
print(VoiceDeliveryReceiptRule.to_json())

# convert the object into a dict
voice_delivery_receipt_rule_dict = voice_delivery_receipt_rule_instance.to_dict()
# create an instance of VoiceDeliveryReceiptRule from a dict
voice_delivery_receipt_rule_from_dict = VoiceDeliveryReceiptRule.from_dict(voice_delivery_receipt_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


