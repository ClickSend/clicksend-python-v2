# DeleteReturnAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **List[str]** |  | [optional] 

## Example

```python
from clicksend.models.delete_return_address import DeleteReturnAddress

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteReturnAddress from a JSON string
delete_return_address_instance = DeleteReturnAddress.from_json(json)
# print the JSON string representation of the object
print(DeleteReturnAddress.to_json())

# convert the object into a dict
delete_return_address_dict = delete_return_address_instance.to_dict()
# create an instance of DeleteReturnAddress from a dict
delete_return_address_from_dict = DeleteReturnAddress.from_dict(delete_return_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


