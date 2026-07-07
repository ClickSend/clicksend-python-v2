# CreateTestInboundSms


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**InboundSmsTest**](InboundSmsTest.md) |  | [optional] 

## Example

```python
from clicksend.models.create_test_inbound_sms import CreateTestInboundSms

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTestInboundSms from a JSON string
create_test_inbound_sms_instance = CreateTestInboundSms.from_json(json)
# print the JSON string representation of the object
print(CreateTestInboundSms.to_json())

# convert the object into a dict
create_test_inbound_sms_dict = create_test_inbound_sms_instance.to_dict()
# create an instance of CreateTestInboundSms from a dict
create_test_inbound_sms_from_dict = CreateTestInboundSms.from_dict(create_test_inbound_sms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


