# CreateSmsInboundAutomationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dedicated_number** | **str** |  | [optional] 
**rule_name** | **str** |  | [optional] 
**message_search_type** | **int** |  | [optional] 
**message_search_term** | **str** |  | [optional] 
**action** | **str** |  | [optional] 
**action_address** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**enabled** | **int** |  | [optional] 

## Example

```python
from clicksend.models.create_sms_inbound_automation_request import CreateSmsInboundAutomationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSmsInboundAutomationRequest from a JSON string
create_sms_inbound_automation_request_instance = CreateSmsInboundAutomationRequest.from_json(json)
# print the JSON string representation of the object
print(CreateSmsInboundAutomationRequest.to_json())

# convert the object into a dict
create_sms_inbound_automation_request_dict = create_sms_inbound_automation_request_instance.to_dict()
# create an instance of CreateSmsInboundAutomationRequest from a dict
create_sms_inbound_automation_request_from_dict = CreateSmsInboundAutomationRequest.from_dict(create_sms_inbound_automation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


