# ViewTemplateCategoriesDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_id** | **float** | The ID of the category. | [optional] 
**category_name** | **str** | The name of the category. | [optional] 

## Example

```python
from clicksend.models.view_template_categories_data_inner import ViewTemplateCategoriesDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewTemplateCategoriesDataInner from a JSON string
view_template_categories_data_inner_instance = ViewTemplateCategoriesDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewTemplateCategoriesDataInner.to_json())

# convert the object into a dict
view_template_categories_data_inner_dict = view_template_categories_data_inner_instance.to_dict()
# create an instance of ViewTemplateCategoriesDataInner from a dict
view_template_categories_data_inner_from_dict = ViewTemplateCategoriesDataInner.from_dict(view_template_categories_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


