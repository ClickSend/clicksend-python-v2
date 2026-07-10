# CreateSmsTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SmsTemplate**](SmsTemplate.md) |  | [optional] 

## Example

```python
from clicksend.models.create_sms_template import CreateSmsTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSmsTemplate from a JSON string
create_sms_template_instance = CreateSmsTemplate.from_json(json)
# print the JSON string representation of the object
print(CreateSmsTemplate.to_json())

# convert the object into a dict
create_sms_template_dict = create_sms_template_instance.to_dict()
# create an instance of CreateSmsTemplate from a dict
create_sms_template_from_dict = CreateSmsTemplate.from_dict(create_sms_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


