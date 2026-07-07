# ViewInboundSms


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewInboundSmsData**](ViewInboundSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_inbound_sms import ViewInboundSms

# TODO update the JSON string below
json = "{}"
# create an instance of ViewInboundSms from a JSON string
view_inbound_sms_instance = ViewInboundSms.from_json(json)
# print the JSON string representation of the object
print(ViewInboundSms.to_json())

# convert the object into a dict
view_inbound_sms_dict = view_inbound_sms_instance.to_dict()
# create an instance of ViewInboundSms from a dict
view_inbound_sms_from_dict = ViewInboundSms.from_dict(view_inbound_sms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


