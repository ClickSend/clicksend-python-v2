# MarkSpecificInboundSmsMessageAsRead


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **int** | The number of SMS marked as read.  If you have multiple inbound rules set to POLL, you will receive the inbound message multiple times. Reading it will mark all those messages as read. | [optional] 

## Example

```python
from clicksend.models.mark_specific_inbound_sms_message_as_read import MarkSpecificInboundSmsMessageAsRead

# TODO update the JSON string below
json = "{}"
# create an instance of MarkSpecificInboundSmsMessageAsRead from a JSON string
mark_specific_inbound_sms_message_as_read_instance = MarkSpecificInboundSmsMessageAsRead.from_json(json)
# print the JSON string representation of the object
print(MarkSpecificInboundSmsMessageAsRead.to_json())

# convert the object into a dict
mark_specific_inbound_sms_message_as_read_dict = mark_specific_inbound_sms_message_as_read_instance.to_dict()
# create an instance of MarkSpecificInboundSmsMessageAsRead from a dict
mark_specific_inbound_sms_message_as_read_from_dict = MarkSpecificInboundSmsMessageAsRead.from_dict(mark_specific_inbound_sms_message_as_read_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


