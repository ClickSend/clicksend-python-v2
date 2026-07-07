# UpdateSmsInboundAutomation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SmsInboundRule**](SmsInboundRule.md) |  | [optional] 

## Example

```python
from clicksend.models.update_sms_inbound_automation import UpdateSmsInboundAutomation

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSmsInboundAutomation from a JSON string
update_sms_inbound_automation_instance = UpdateSmsInboundAutomation.from_json(json)
# print the JSON string representation of the object
print(UpdateSmsInboundAutomation.to_json())

# convert the object into a dict
update_sms_inbound_automation_dict = update_sms_inbound_automation_instance.to_dict()
# create an instance of UpdateSmsInboundAutomation from a dict
update_sms_inbound_automation_from_dict = UpdateSmsInboundAutomation.from_dict(update_sms_inbound_automation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


