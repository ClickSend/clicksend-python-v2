# UpdateReturnAddressRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_country** | **str** |  | [optional] 
**address_state** | **str** |  | [optional] 

## Example

```python
from clicksend.models.update_return_address_request import UpdateReturnAddressRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateReturnAddressRequest from a JSON string
update_return_address_request_instance = UpdateReturnAddressRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateReturnAddressRequest.to_json())

# convert the object into a dict
update_return_address_request_dict = update_return_address_request_instance.to_dict()
# create an instance of UpdateReturnAddressRequest from a dict
update_return_address_request_from_dict = UpdateReturnAddressRequest.from_dict(update_return_address_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


