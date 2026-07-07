# CalculateFaxPriceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_url** | **str** |  | [optional] 
**messages** | [**List[CalculateFaxPriceRequestMessagesInner]**](CalculateFaxPriceRequestMessagesInner.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_fax_price_request import CalculateFaxPriceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateFaxPriceRequest from a JSON string
calculate_fax_price_request_instance = CalculateFaxPriceRequest.from_json(json)
# print the JSON string representation of the object
print(CalculateFaxPriceRequest.to_json())

# convert the object into a dict
calculate_fax_price_request_dict = calculate_fax_price_request_instance.to_dict()
# create an instance of CalculateFaxPriceRequest from a dict
calculate_fax_price_request_from_dict = CalculateFaxPriceRequest.from_dict(calculate_fax_price_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


