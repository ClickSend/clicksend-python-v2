# BuyNumberRequestRegistrationData

Optional registration data for number compliance

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**business_name** | **str** | Name of the business (2 - 100 characters) | 
**business_address** | **str** | Business address (5 - 150 characters) | 
**suburb** | **str** | Suburb/City (2 - 50 characters) | 
**postcode** | **str** | Postal code (2 - 20 characters) | 
**state** | **str** | State/Province (2 - 50 characters) | 
**contact_name** | **str** | Contact person name (2 - 100 characters) | 
**contact_number** | **str** | Contact phone number (valid local or international phone number) | 
**country** | **str** | Country code (ISO 3166-1 alpha-2) | 

## Example

```python
from clicksend.models.buy_number_request_registration_data import BuyNumberRequestRegistrationData

# TODO update the JSON string below
json = "{}"
# create an instance of BuyNumberRequestRegistrationData from a JSON string
buy_number_request_registration_data_instance = BuyNumberRequestRegistrationData.from_json(json)
# print the JSON string representation of the object
print(BuyNumberRequestRegistrationData.to_json())

# convert the object into a dict
buy_number_request_registration_data_dict = buy_number_request_registration_data_instance.to_dict()
# create an instance of BuyNumberRequestRegistrationData from a dict
buy_number_request_registration_data_from_dict = BuyNumberRequestRegistrationData.from_dict(buy_number_request_registration_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


