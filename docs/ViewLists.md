# ViewLists


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewListsData**](ViewListsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_lists import ViewLists

# TODO update the JSON string below
json = "{}"
# create an instance of ViewLists from a JSON string
view_lists_instance = ViewLists.from_json(json)
# print the JSON string representation of the object
print(ViewLists.to_json())

# convert the object into a dict
view_lists_dict = view_lists_instance.to_dict()
# create an instance of ViewLists from a dict
view_lists_from_dict = ViewLists.from_dict(view_lists_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


