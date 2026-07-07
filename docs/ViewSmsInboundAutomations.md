# ViewSmsInboundAutomations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewSmsInboundAutomationsData**](ViewSmsInboundAutomationsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_inbound_automations import ViewSmsInboundAutomations

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsInboundAutomations from a JSON string
view_sms_inbound_automations_instance = ViewSmsInboundAutomations.from_json(json)
# print the JSON string representation of the object
print(ViewSmsInboundAutomations.to_json())

# convert the object into a dict
view_sms_inbound_automations_dict = view_sms_inbound_automations_instance.to_dict()
# create an instance of ViewSmsInboundAutomations from a dict
view_sms_inbound_automations_from_dict = ViewSmsInboundAutomations.from_dict(view_sms_inbound_automations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


