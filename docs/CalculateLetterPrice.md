# CalculateLetterPrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CalculateLetterPriceData**](CalculateLetterPriceData.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_letter_price import CalculateLetterPrice

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateLetterPrice from a JSON string
calculate_letter_price_instance = CalculateLetterPrice.from_json(json)
# print the JSON string representation of the object
print(CalculateLetterPrice.to_json())

# convert the object into a dict
calculate_letter_price_dict = calculate_letter_price_instance.to_dict()
# create an instance of CalculateLetterPrice from a dict
calculate_letter_price_from_dict = CalculateLetterPrice.from_dict(calculate_letter_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


