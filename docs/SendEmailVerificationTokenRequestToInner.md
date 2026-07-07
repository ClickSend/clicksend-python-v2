# SendEmailVerificationTokenRequestToInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_email_verification_token_request_to_inner import SendEmailVerificationTokenRequestToInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailVerificationTokenRequestToInner from a JSON string
send_email_verification_token_request_to_inner_instance = SendEmailVerificationTokenRequestToInner.from_json(json)
# print the JSON string representation of the object
print(SendEmailVerificationTokenRequestToInner.to_json())

# convert the object into a dict
send_email_verification_token_request_to_inner_dict = send_email_verification_token_request_to_inner_instance.to_dict()
# create an instance of SendEmailVerificationTokenRequestToInner from a dict
send_email_verification_token_request_to_inner_from_dict = SendEmailVerificationTokenRequestToInner.from_dict(send_email_verification_token_request_to_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


