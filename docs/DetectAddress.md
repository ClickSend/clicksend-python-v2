# DetectAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**DetectAddressData**](DetectAddressData.md) |  | [optional] 

## Example

```python
from clicksend.models.detect_address import DetectAddress

# TODO update the JSON string below
json = "{}"
# create an instance of DetectAddress from a JSON string
detect_address_instance = DetectAddress.from_json(json)
# print the JSON string representation of the object
print(DetectAddress.to_json())

# convert the object into a dict
detect_address_dict = detect_address_instance.to_dict()
# create an instance of DetectAddress from a dict
detect_address_from_dict = DetectAddress.from_dict(detect_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


