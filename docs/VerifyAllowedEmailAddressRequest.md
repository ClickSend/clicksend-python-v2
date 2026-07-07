# VerifyAllowedEmailAddressRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | [**List[SendEmailRequestToInner]**](SendEmailRequestToInner.md) |  | [optional] 
**var_from** | [**SendEmailVerificationTokenRequestFrom**](SendEmailVerificationTokenRequestFrom.md) |  | [optional] 
**subject** | **str** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from clicksend.models.verify_allowed_email_address_request import VerifyAllowedEmailAddressRequest

# TODO update the JSON string below
json = "{}"
# create an instance of VerifyAllowedEmailAddressRequest from a JSON string
verify_allowed_email_address_request_instance = VerifyAllowedEmailAddressRequest.from_json(json)
# print the JSON string representation of the object
print(VerifyAllowedEmailAddressRequest.to_json())

# convert the object into a dict
verify_allowed_email_address_request_dict = verify_allowed_email_address_request_instance.to_dict()
# create an instance of VerifyAllowedEmailAddressRequest from a dict
verify_allowed_email_address_request_from_dict = VerifyAllowedEmailAddressRequest.from_dict(verify_allowed_email_address_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


