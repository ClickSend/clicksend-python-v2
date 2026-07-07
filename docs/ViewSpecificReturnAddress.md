# ViewSpecificReturnAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**PostReturnAddress**](PostReturnAddress.md) |  | [optional] 

## Example

```python
from clicksend.models.view_specific_return_address import ViewSpecificReturnAddress

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSpecificReturnAddress from a JSON string
view_specific_return_address_instance = ViewSpecificReturnAddress.from_json(json)
# print the JSON string representation of the object
print(ViewSpecificReturnAddress.to_json())

# convert the object into a dict
view_specific_return_address_dict = view_specific_return_address_instance.to_dict()
# create an instance of ViewSpecificReturnAddress from a dict
view_specific_return_address_from_dict = ViewSpecificReturnAddress.from_dict(view_specific_return_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


