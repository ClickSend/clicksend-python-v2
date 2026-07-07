# SendEmailVerificationTokenRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | [**List[SendEmailVerificationTokenRequestToInner]**](SendEmailVerificationTokenRequestToInner.md) |  | [optional] 
**var_from** | [**SendEmailVerificationTokenRequestFrom**](SendEmailVerificationTokenRequestFrom.md) |  | [optional] 
**subject** | **str** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_email_verification_token_request import SendEmailVerificationTokenRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailVerificationTokenRequest from a JSON string
send_email_verification_token_request_instance = SendEmailVerificationTokenRequest.from_json(json)
# print the JSON string representation of the object
print(SendEmailVerificationTokenRequest.to_json())

# convert the object into a dict
send_email_verification_token_request_dict = send_email_verification_token_request_instance.to_dict()
# create an instance of SendEmailVerificationTokenRequest from a dict
send_email_verification_token_request_from_dict = SendEmailVerificationTokenRequest.from_dict(send_email_verification_token_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


