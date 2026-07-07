# BuyNumberRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dedicated_number** | **str** | Phone number to purchase | 
**type** | **str** | Service type for the number | 
**registration_data** | [**BuyNumberRequestRegistrationData**](BuyNumberRequestRegistrationData.md) |  | [optional] 

## Example

```python
from clicksend.models.buy_number_request import BuyNumberRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BuyNumberRequest from a JSON string
buy_number_request_instance = BuyNumberRequest.from_json(json)
# print the JSON string representation of the object
print(BuyNumberRequest.to_json())

# convert the object into a dict
buy_number_request_dict = buy_number_request_instance.to_dict()
# create an instance of BuyNumberRequest from a dict
buy_number_request_from_dict = BuyNumberRequest.from_dict(buy_number_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


