# VerifyAllowedEmailAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**EmailAddress**](EmailAddress.md) |  | [optional] 

## Example

```python
from clicksend.models.verify_allowed_email_address import VerifyAllowedEmailAddress

# TODO update the JSON string below
json = "{}"
# create an instance of VerifyAllowedEmailAddress from a JSON string
verify_allowed_email_address_instance = VerifyAllowedEmailAddress.from_json(json)
# print the JSON string representation of the object
print(VerifyAllowedEmailAddress.to_json())

# convert the object into a dict
verify_allowed_email_address_dict = verify_allowed_email_address_instance.to_dict()
# create an instance of VerifyAllowedEmailAddress from a dict
verify_allowed_email_address_from_dict = VerifyAllowedEmailAddress.from_dict(verify_allowed_email_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


