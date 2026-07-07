# ViewEmailTemplatesDataDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **int** | The ID of the email template. | [optional] 
**template_name** | **str** | The name of the email template. | [optional] 

## Example

```python
from clicksend.models.view_email_templates_data_data_inner import ViewEmailTemplatesDataDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewEmailTemplatesDataDataInner from a JSON string
view_email_templates_data_data_inner_instance = ViewEmailTemplatesDataDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewEmailTemplatesDataDataInner.to_json())

# convert the object into a dict
view_email_templates_data_data_inner_dict = view_email_templates_data_data_inner_instance.to_dict()
# create an instance of ViewEmailTemplatesDataDataInner from a dict
view_email_templates_data_data_inner_from_dict = ViewEmailTemplatesDataDataInner.from_dict(view_email_templates_data_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


