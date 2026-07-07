# ViewSmsInboundAutomation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SmsInboundRule**](SmsInboundRule.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_inbound_automation import ViewSmsInboundAutomation

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsInboundAutomation from a JSON string
view_sms_inbound_automation_instance = ViewSmsInboundAutomation.from_json(json)
# print the JSON string representation of the object
print(ViewSmsInboundAutomation.to_json())

# convert the object into a dict
view_sms_inbound_automation_dict = view_sms_inbound_automation_instance.to_dict()
# create an instance of ViewSmsInboundAutomation from a dict
view_sms_inbound_automation_from_dict = ViewSmsInboundAutomation.from_dict(view_sms_inbound_automation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


