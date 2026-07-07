# ViewASpecificInboundSmsMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**InboundSms**](InboundSms.md) |  | [optional] 

## Example

```python
from clicksend.models.view_a_specific_inbound_sms_message import ViewASpecificInboundSmsMessage

# TODO update the JSON string below
json = "{}"
# create an instance of ViewASpecificInboundSmsMessage from a JSON string
view_a_specific_inbound_sms_message_instance = ViewASpecificInboundSmsMessage.from_json(json)
# print the JSON string representation of the object
print(ViewASpecificInboundSmsMessage.to_json())

# convert the object into a dict
view_a_specific_inbound_sms_message_dict = view_a_specific_inbound_sms_message_instance.to_dict()
# create an instance of ViewASpecificInboundSmsMessage from a dict
view_a_specific_inbound_sms_message_from_dict = ViewASpecificInboundSmsMessage.from_dict(view_a_specific_inbound_sms_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


