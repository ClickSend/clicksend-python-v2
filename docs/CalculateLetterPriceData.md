# CalculateLetterPriceData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_price** | **float** | The total price of the letter. | [optional] 
**total_cost** | **float** | The total cost of the letter. | [optional] 
**recipients** | [**List[Recipient]**](Recipient.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_letter_price_data import CalculateLetterPriceData

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateLetterPriceData from a JSON string
calculate_letter_price_data_instance = CalculateLetterPriceData.from_json(json)
# print the JSON string representation of the object
print(CalculateLetterPriceData.to_json())

# convert the object into a dict
calculate_letter_price_data_dict = calculate_letter_price_data_instance.to_dict()
# create an instance of CalculateLetterPriceData from a dict
calculate_letter_price_data_from_dict = CalculateLetterPriceData.from_dict(calculate_letter_price_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


