# InboundFaxRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**inbound_rule_id** | **int** | The ID of the inbound rule | [optional] 
**dedicated_number** | **str** | The dedicated number | [optional] 
**rule_name** | **str** | The name of the inbound rule | [optional] 
**user_id** | **int** | The ID of the user | [optional] 
**action** | **str** | The action | [optional] 
**action_address** | **str** | The address associated with the action | [optional] 
**enabled** | **int** | Indicates whether the rule is enabled | [optional] 

## Example

```python
from clicksend.models.inbound_fax_rule import InboundFaxRule

# TODO update the JSON string below
json = "{}"
# create an instance of InboundFaxRule from a JSON string
inbound_fax_rule_instance = InboundFaxRule.from_json(json)
# print the JSON string representation of the object
print(InboundFaxRule.to_json())

# convert the object into a dict
inbound_fax_rule_dict = inbound_fax_rule_instance.to_dict()
# create an instance of InboundFaxRule from a dict
inbound_fax_rule_from_dict = InboundFaxRule.from_dict(inbound_fax_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


