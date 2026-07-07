# UpdateSmsInboundAutomationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dedicated_number** | **str** |  | [optional] 
**rule_name** | **str** |  | [optional] 
**message_search_type** | **int** |  | [optional] 
**message_search_term** | **str** |  | [optional] 
**action** | **str** |  | [optional] 
**action_address** | **str** |  | [optional] 
**enabled** | **int** |  | [optional] 

## Example

```python
from clicksend.models.update_sms_inbound_automation_request import UpdateSmsInboundAutomationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSmsInboundAutomationRequest from a JSON string
update_sms_inbound_automation_request_instance = UpdateSmsInboundAutomationRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateSmsInboundAutomationRequest.to_json())

# convert the object into a dict
update_sms_inbound_automation_request_dict = update_sms_inbound_automation_request_instance.to_dict()
# create an instance of UpdateSmsInboundAutomationRequest from a dict
update_sms_inbound_automation_request_from_dict = UpdateSmsInboundAutomationRequest.from_dict(update_sms_inbound_automation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


