# SmsTemplateUpdate

The parameters related to the actual templates.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **int** | The generated ID of the template. This remains the same and can’t be updated. | [optional] 
**body** | **str** | The new updated content of the template. | [optional] 
**template_name** | **str** | The new updated name of the template. | [optional] 

## Example

```python
from clicksend.models.sms_template_update import SmsTemplateUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of SmsTemplateUpdate from a JSON string
sms_template_update_instance = SmsTemplateUpdate.from_json(json)
# print the JSON string representation of the object
print(SmsTemplateUpdate.to_json())

# convert the object into a dict
sms_template_update_dict = sms_template_update_instance.to_dict()
# create an instance of SmsTemplateUpdate from a dict
sms_template_update_from_dict = SmsTemplateUpdate.from_dict(sms_template_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


