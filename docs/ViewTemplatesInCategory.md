# ViewTemplatesInCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[MasterEmailTemplate]**](MasterEmailTemplate.md) |  | [optional] 

## Example

```python
from clicksend.models.view_templates_in_category import ViewTemplatesInCategory

# TODO update the JSON string below
json = "{}"
# create an instance of ViewTemplatesInCategory from a JSON string
view_templates_in_category_instance = ViewTemplatesInCategory.from_json(json)
# print the JSON string representation of the object
print(ViewTemplatesInCategory.to_json())

# convert the object into a dict
view_templates_in_category_dict = view_templates_in_category_instance.to_dict()
# create an instance of ViewTemplatesInCategory from a dict
view_templates_in_category_from_dict = ViewTemplatesInCategory.from_dict(view_templates_in_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


