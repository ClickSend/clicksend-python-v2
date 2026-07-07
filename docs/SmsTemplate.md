# SmsTemplate

The parameters related to the actual templates.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **int** | The generated ID of the template. | [optional] 
**body** | **str** | The main content of the template. | [optional] 
**template_name** | **str** | The name of the template. | [optional] 

## Example

```python
from clicksend.models.sms_template import SmsTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of SmsTemplate from a JSON string
sms_template_instance = SmsTemplate.from_json(json)
# print the JSON string representation of the object
print(SmsTemplate.to_json())

# convert the object into a dict
sms_template_dict = sms_template_instance.to_dict()
# create an instance of SmsTemplate from a dict
sms_template_from_dict = SmsTemplate.from_dict(sms_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


