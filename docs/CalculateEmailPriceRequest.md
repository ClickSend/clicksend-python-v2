# CalculateEmailPriceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | [**List[SendEmailRequestToInner]**](SendEmailRequestToInner.md) |  | [optional] 
**var_from** | [**SendEmailRequestFrom**](SendEmailRequestFrom.md) |  | [optional] 
**subject** | **str** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from clicksend.models.calculate_email_price_request import CalculateEmailPriceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateEmailPriceRequest from a JSON string
calculate_email_price_request_instance = CalculateEmailPriceRequest.from_json(json)
# print the JSON string representation of the object
print(CalculateEmailPriceRequest.to_json())

# convert the object into a dict
calculate_email_price_request_dict = calculate_email_price_request_instance.to_dict()
# create an instance of CalculateEmailPriceRequest from a dict
calculate_email_price_request_from_dict = CalculateEmailPriceRequest.from_dict(calculate_email_price_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


