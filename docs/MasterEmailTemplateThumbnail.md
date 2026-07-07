# MasterEmailTemplateThumbnail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**small** | **str** | The small thumbnail of the template. | [optional] 
**large** | **str** | The large thumbnail of the template. | [optional] 

## Example

```python
from clicksend.models.master_email_template_thumbnail import MasterEmailTemplateThumbnail

# TODO update the JSON string below
json = "{}"
# create an instance of MasterEmailTemplateThumbnail from a JSON string
master_email_template_thumbnail_instance = MasterEmailTemplateThumbnail.from_json(json)
# print the JSON string representation of the object
print(MasterEmailTemplateThumbnail.to_json())

# convert the object into a dict
master_email_template_thumbnail_dict = master_email_template_thumbnail_instance.to_dict()
# create an instance of MasterEmailTemplateThumbnail from a dict
master_email_template_thumbnail_from_dict = MasterEmailTemplateThumbnail.from_dict(master_email_template_thumbnail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


