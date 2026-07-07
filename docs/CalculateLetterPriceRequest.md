# CalculateLetterPriceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_url** | **str** |  | [optional] 
**template_used** | **int** |  | [optional] 
**duplex** | **int** |  | [optional] 
**colour** | **int** |  | [optional] 
**source** | **str** |  | [optional] 
**recipients** | [**List[SendPostcardRequestRecipientsInner]**](SendPostcardRequestRecipientsInner.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_letter_price_request import CalculateLetterPriceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateLetterPriceRequest from a JSON string
calculate_letter_price_request_instance = CalculateLetterPriceRequest.from_json(json)
# print the JSON string representation of the object
print(CalculateLetterPriceRequest.to_json())

# convert the object into a dict
calculate_letter_price_request_dict = calculate_letter_price_request_instance.to_dict()
# create an instance of CalculateLetterPriceRequest from a dict
calculate_letter_price_request_from_dict = CalculateLetterPriceRequest.from_dict(calculate_letter_price_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


