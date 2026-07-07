# MasterEmailTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id_master** | **int** | The unique identifier for the template. | [optional] 
**template_name** | **str** | The name of the template. | [optional] 
**date_added** | **str** | The date the template was added. | [optional] 
**body** | **str** | The body of the template. | [optional] 
**thumbnail** | [**MasterEmailTemplateThumbnail**](MasterEmailTemplateThumbnail.md) |  | [optional] 

## Example

```python
from clicksend.models.master_email_template import MasterEmailTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of MasterEmailTemplate from a JSON string
master_email_template_instance = MasterEmailTemplate.from_json(json)
# print the JSON string representation of the object
print(MasterEmailTemplate.to_json())

# convert the object into a dict
master_email_template_dict = master_email_template_instance.to_dict()
# create an instance of MasterEmailTemplate from a dict
master_email_template_from_dict = MasterEmailTemplate.from_dict(master_email_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


