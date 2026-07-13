# SendSms


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information.  This parameter doesn’t reflect the status of each message. Check the status parameter of the message object to view the status of the individual message. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SendSmsData**](SendSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.send_sms import SendSms

# TODO update the JSON string below
json = "{}"
# create an instance of SendSms from a JSON string
send_sms_instance = SendSms.from_json(json)
# print the JSON string representation of the object
print(SendSms.to_json())

# convert the object into a dict
send_sms_dict = send_sms_instance.to_dict()
# create an instance of SendSms from a dict
send_sms_from_dict = SendSms.from_dict(send_sms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


