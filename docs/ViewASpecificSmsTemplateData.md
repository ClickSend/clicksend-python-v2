# ViewASpecificSmsTemplateData

The parameters related to the template.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **int** | The generated ID of the template. | [optional] 
**template_name** | **str** | The main content of the template. | [optional] 
**body** | **str** | The name of the template. | [optional] 

## Example

```python
from clicksend.models.view_a_specific_sms_template_data import ViewASpecificSmsTemplateData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewASpecificSmsTemplateData from a JSON string
view_a_specific_sms_template_data_instance = ViewASpecificSmsTemplateData.from_json(json)
# print the JSON string representation of the object
print(ViewASpecificSmsTemplateData.to_json())

# convert the object into a dict
view_a_specific_sms_template_data_dict = view_a_specific_sms_template_data_instance.to_dict()
# create an instance of ViewASpecificSmsTemplateData from a dict
view_a_specific_sms_template_data_from_dict = ViewASpecificSmsTemplateData.from_dict(view_a_specific_sms_template_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


