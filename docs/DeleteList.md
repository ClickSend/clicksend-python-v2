# DeleteList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **List[str]** |  | [optional] 

## Example

```python
from clicksend.models.delete_list import DeleteList

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteList from a JSON string
delete_list_instance = DeleteList.from_json(json)
# print the JSON string representation of the object
print(DeleteList.to_json())

# convert the object into a dict
delete_list_dict = delete_list_instance.to_dict()
# create an instance of DeleteList from a dict
delete_list_from_dict = DeleteList.from_dict(delete_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


