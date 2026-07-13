# UpdateSmsTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SmsTemplateUpdate**](SmsTemplateUpdate.md) |  | [optional] 

## Example

```python
from clicksend.models.update_sms_template import UpdateSmsTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSmsTemplate from a JSON string
update_sms_template_instance = UpdateSmsTemplate.from_json(json)
# print the JSON string representation of the object
print(UpdateSmsTemplate.to_json())

# convert the object into a dict
update_sms_template_dict = update_sms_template_instance.to_dict()
# create an instance of UpdateSmsTemplate from a dict
update_sms_template_from_dict = UpdateSmsTemplate.from_dict(update_sms_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


