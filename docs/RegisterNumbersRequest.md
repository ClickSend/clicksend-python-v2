# RegisterNumbersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**full_name** | **str** | Legal full name of the individual registering the number. Must be a personal name, not a business name. | 
**company_name** | **str** | Legal business name of the organization requesting registration | 
**email** | **str** | Contact email address for registration communications and notifications | 
**website_url** | **str** | Official business website URL | 
**sample_message** | **str** | Representative example of messages that will be sent using this number | 
**primary_use_case** | **str** | Primary intended purpose for the registered number (e.g., Marketing, Notifications, Authentication) | 
**company_number** | **str** | Official support phone number of the organization requesting registration | 
**area_code** | **str** | Your area codes, please provide your top 3 area codes in case your 1st choice is not available | 

## Example

```python
from clicksend.models.register_numbers_request import RegisterNumbersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RegisterNumbersRequest from a JSON string
register_numbers_request_instance = RegisterNumbersRequest.from_json(json)
# print the JSON string representation of the object
print(RegisterNumbersRequest.to_json())

# convert the object into a dict
register_numbers_request_dict = register_numbers_request_instance.to_dict()
# create an instance of RegisterNumbersRequest from a dict
register_numbers_request_from_dict = RegisterNumbersRequest.from_dict(register_numbers_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


