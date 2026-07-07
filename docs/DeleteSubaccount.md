# DeleteSubaccount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **bool** | The status of the operation. | [optional] 

## Example

```python
from clicksend.models.delete_subaccount import DeleteSubaccount

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteSubaccount from a JSON string
delete_subaccount_instance = DeleteSubaccount.from_json(json)
# print the JSON string representation of the object
print(DeleteSubaccount.to_json())

# convert the object into a dict
delete_subaccount_dict = delete_subaccount_instance.to_dict()
# create an instance of DeleteSubaccount from a dict
delete_subaccount_from_dict = DeleteSubaccount.from_dict(delete_subaccount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


