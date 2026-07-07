# CalculateVoicePriceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**messages** | [**List[CalculateVoicePriceRequestMessagesInner]**](CalculateVoicePriceRequestMessagesInner.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_voice_price_request import CalculateVoicePriceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateVoicePriceRequest from a JSON string
calculate_voice_price_request_instance = CalculateVoicePriceRequest.from_json(json)
# print the JSON string representation of the object
print(CalculateVoicePriceRequest.to_json())

# convert the object into a dict
calculate_voice_price_request_dict = calculate_voice_price_request_instance.to_dict()
# create an instance of CalculateVoicePriceRequest from a dict
calculate_voice_price_request_from_dict = CalculateVoicePriceRequest.from_dict(calculate_voice_price_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


