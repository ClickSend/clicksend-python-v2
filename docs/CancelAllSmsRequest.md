# CancelAllSmsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custom_string** | **str** | The scheduled messages to cancel with the specified _custom_string_. When you send an SMS, you can add an optional _custom_string_ to it. This parameter allows you to cancel messages that have this _custom_string_.  It&#39;s commonly used for canceling scheduled [SMS campaigns](/messaging/sms-campaigns/). When you send an SMS campaign, the system automatically adds a _custom_string_ to each message, and this parameter lets you cancel only those specific messages. | [optional] 

## Example

```python
from clicksend.models.cancel_all_sms_request import CancelAllSmsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CancelAllSmsRequest from a JSON string
cancel_all_sms_request_instance = CancelAllSmsRequest.from_json(json)
# print the JSON string representation of the object
print(CancelAllSmsRequest.to_json())

# convert the object into a dict
cancel_all_sms_request_dict = cancel_all_sms_request_instance.to_dict()
# create an instance of CancelAllSmsRequest from a dict
cancel_all_sms_request_from_dict = CancelAllSmsRequest.from_dict(cancel_all_sms_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


