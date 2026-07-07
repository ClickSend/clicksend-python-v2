# CreateAllowedEmailAddressRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address** | **str** |  | [optional] 

## Example

```python
from clicksend.models.create_allowed_email_address_request import CreateAllowedEmailAddressRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAllowedEmailAddressRequest from a JSON string
create_allowed_email_address_request_instance = CreateAllowedEmailAddressRequest.from_json(json)
# print the JSON string representation of the object
print(CreateAllowedEmailAddressRequest.to_json())

# convert the object into a dict
create_allowed_email_address_request_dict = create_allowed_email_address_request_instance.to_dict()
# create an instance of CreateAllowedEmailAddressRequest from a dict
create_allowed_email_address_request_from_dict = CreateAllowedEmailAddressRequest.from_dict(create_allowed_email_address_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


