# CalculateMmsPriceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**media_file** | **str** |  | [optional] 
**messages** | [**List[CalculateMmsPriceRequestMessagesInner]**](CalculateMmsPriceRequestMessagesInner.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_mms_price_request import CalculateMmsPriceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateMmsPriceRequest from a JSON string
calculate_mms_price_request_instance = CalculateMmsPriceRequest.from_json(json)
# print the JSON string representation of the object
print(CalculateMmsPriceRequest.to_json())

# convert the object into a dict
calculate_mms_price_request_dict = calculate_mms_price_request_instance.to_dict()
# create an instance of CalculateMmsPriceRequest from a dict
calculate_mms_price_request_from_dict = CalculateMmsPriceRequest.from_dict(calculate_mms_price_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


