# SmsInboundRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**inbound_rule_id** | **int** | The ID of the inbound rule. | [optional] 
**dedicated_number** | **str** | The number to be used in the inbound rule. | [optional] 
**rule_name** | **str** | The name of the inbound rule. | [optional] 
**message_search_type** | **int** | The type of message search to be used in the inbound rule. | [optional] 
**message_search_term** | **str** | The message search term to be used in the inbound rule. | [optional] 
**action** | **str** | The action to be taken in the inbound rule. | [optional] 
**action_address** | **str** | The action address to be used in the inbound rule. | [optional] 
**body** | **str** | The body of the inbound rule. | [optional] 
**enabled** | **int** | The status of the inbound rule. | [optional] 
**webhook_type** | **str** | The format used when calling the webhook (e.g. post, json). | [optional] 

## Example

```python
from clicksend.models.sms_inbound_rule import SmsInboundRule

# TODO update the JSON string below
json = "{}"
# create an instance of SmsInboundRule from a JSON string
sms_inbound_rule_instance = SmsInboundRule.from_json(json)
# print the JSON string representation of the object
print(SmsInboundRule.to_json())

# convert the object into a dict
sms_inbound_rule_dict = sms_inbound_rule_instance.to_dict()
# create an instance of SmsInboundRule from a dict
sms_inbound_rule_from_dict = SmsInboundRule.from_dict(sms_inbound_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


