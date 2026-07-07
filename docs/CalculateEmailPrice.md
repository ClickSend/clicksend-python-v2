# CalculateEmailPrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CalculateEmailPriceData**](CalculateEmailPriceData.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_email_price import CalculateEmailPrice

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateEmailPrice from a JSON string
calculate_email_price_instance = CalculateEmailPrice.from_json(json)
# print the JSON string representation of the object
print(CalculateEmailPrice.to_json())

# convert the object into a dict
calculate_email_price_dict = calculate_email_price_instance.to_dict()
# create an instance of CalculateEmailPrice from a dict
calculate_email_price_from_dict = CalculateEmailPrice.from_dict(calculate_email_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


