# CreateReturnAddressRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_name** | **str** |  | [optional] 
**address_line_1** | **str** |  | [optional] 
**address_line_2** | **str** |  | [optional] 
**address_city** | **str** |  | [optional] 
**address_postal_code** | **str** |  | [optional] 
**address_country** | **str** |  | [optional] 

## Example

```python
from clicksend.models.create_return_address_request import CreateReturnAddressRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateReturnAddressRequest from a JSON string
create_return_address_request_instance = CreateReturnAddressRequest.from_json(json)
# print the JSON string representation of the object
print(CreateReturnAddressRequest.to_json())

# convert the object into a dict
create_return_address_request_dict = create_return_address_request_instance.to_dict()
# create an instance of CreateReturnAddressRequest from a dict
create_return_address_request_from_dict = CreateReturnAddressRequest.from_dict(create_return_address_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


