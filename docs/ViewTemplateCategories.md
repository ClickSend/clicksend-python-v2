# ViewTemplateCategories


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[ViewTemplateCategoriesDataInner]**](ViewTemplateCategoriesDataInner.md) |  | [optional] 

## Example

```python
from clicksend.models.view_template_categories import ViewTemplateCategories

# TODO update the JSON string below
json = "{}"
# create an instance of ViewTemplateCategories from a JSON string
view_template_categories_instance = ViewTemplateCategories.from_json(json)
# print the JSON string representation of the object
print(ViewTemplateCategories.to_json())

# convert the object into a dict
view_template_categories_dict = view_template_categories_instance.to_dict()
# create an instance of ViewTemplateCategories from a dict
view_template_categories_from_dict = ViewTemplateCategories.from_dict(view_template_categories_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


