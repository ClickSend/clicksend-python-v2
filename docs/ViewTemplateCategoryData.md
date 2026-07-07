# ViewTemplateCategoryData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_id** | **float** | The ID of the category. | [optional] 
**name** | **str** | The name of the category. | [optional] 

## Example

```python
from clicksend.models.view_template_category_data import ViewTemplateCategoryData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewTemplateCategoryData from a JSON string
view_template_category_data_instance = ViewTemplateCategoryData.from_json(json)
# print the JSON string representation of the object
print(ViewTemplateCategoryData.to_json())

# convert the object into a dict
view_template_category_data_dict = view_template_category_data_instance.to_dict()
# create an instance of ViewTemplateCategoryData from a dict
view_template_category_data_from_dict = ViewTemplateCategoryData.from_dict(view_template_category_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


