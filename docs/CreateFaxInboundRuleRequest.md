# CreateFaxInboundRuleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dedicated_number** | **str** |  | [optional] 
**rule_name** | **str** |  | [optional] 
**action** | **str** |  | [optional] 
**action_address** | **str** |  | [optional] 
**enabled** | **int** |  | [optional] 

## Example

```python
from clicksend.models.create_fax_inbound_rule_request import CreateFaxInboundRuleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateFaxInboundRuleRequest from a JSON string
create_fax_inbound_rule_request_instance = CreateFaxInboundRuleRequest.from_json(json)
# print the JSON string representation of the object
print(CreateFaxInboundRuleRequest.to_json())

# convert the object into a dict
create_fax_inbound_rule_request_dict = create_fax_inbound_rule_request_instance.to_dict()
# create an instance of CreateFaxInboundRuleRequest from a dict
create_fax_inbound_rule_request_from_dict = CreateFaxInboundRuleRequest.from_dict(create_fax_inbound_rule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


