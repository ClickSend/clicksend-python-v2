# UpdateList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ContactList**](ContactList.md) |  | [optional] 

## Example

```python
from clicksend.models.update_list import UpdateList

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateList from a JSON string
update_list_instance = UpdateList.from_json(json)
# print the JSON string representation of the object
print(UpdateList.to_json())

# convert the object into a dict
update_list_dict = update_list_instance.to_dict()
# create an instance of UpdateList from a dict
update_list_from_dict = UpdateList.from_dict(update_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


