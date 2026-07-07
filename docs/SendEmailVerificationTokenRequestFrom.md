# SendEmailVerificationTokenRequestFrom


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_email_verification_token_request_from import SendEmailVerificationTokenRequestFrom

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailVerificationTokenRequestFrom from a JSON string
send_email_verification_token_request_from_instance = SendEmailVerificationTokenRequestFrom.from_json(json)
# print the JSON string representation of the object
print(SendEmailVerificationTokenRequestFrom.to_json())

# convert the object into a dict
send_email_verification_token_request_from_dict = send_email_verification_token_request_from_instance.to_dict()
# create an instance of SendEmailVerificationTokenRequestFrom from a dict
send_email_verification_token_request_from_from_dict = SendEmailVerificationTokenRequestFrom.from_dict(send_email_verification_token_request_from_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


