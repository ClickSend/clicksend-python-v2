# ViewFaxInboundRules


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewFaxInboundRulesData**](ViewFaxInboundRulesData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_fax_inbound_rules import ViewFaxInboundRules

# TODO update the JSON string below
json = "{}"
# create an instance of ViewFaxInboundRules from a JSON string
view_fax_inbound_rules_instance = ViewFaxInboundRules.from_json(json)
# print the JSON string representation of the object
print(ViewFaxInboundRules.to_json())

# convert the object into a dict
view_fax_inbound_rules_dict = view_fax_inbound_rules_instance.to_dict()
# create an instance of ViewFaxInboundRules from a dict
view_fax_inbound_rules_from_dict = ViewFaxInboundRules.from_dict(view_fax_inbound_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


