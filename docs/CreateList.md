# CreateList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ContactList**](ContactList.md) |  | [optional] 

## Example

```python
from clicksend.models.create_list import CreateList

# TODO update the JSON string below
json = "{}"
# create an instance of CreateList from a JSON string
create_list_instance = CreateList.from_json(json)
# print the JSON string representation of the object
print(CreateList.to_json())

# convert the object into a dict
create_list_dict = create_list_instance.to_dict()
# create an instance of CreateList from a dict
create_list_from_dict = CreateList.from_dict(create_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


