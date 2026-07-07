# ViewYourReturnAddresses


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewYourReturnAddressesData**](ViewYourReturnAddressesData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_your_return_addresses import ViewYourReturnAddresses

# TODO update the JSON string below
json = "{}"
# create an instance of ViewYourReturnAddresses from a JSON string
view_your_return_addresses_instance = ViewYourReturnAddresses.from_json(json)
# print the JSON string representation of the object
print(ViewYourReturnAddresses.to_json())

# convert the object into a dict
view_your_return_addresses_dict = view_your_return_addresses_instance.to_dict()
# create an instance of ViewYourReturnAddresses from a dict
view_your_return_addresses_from_dict = ViewYourReturnAddresses.from_dict(view_your_return_addresses_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


