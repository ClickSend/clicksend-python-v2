# ForgotUsernameRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | [optional] 

## Example

```python
from clicksend.models.forgot_username_request import ForgotUsernameRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ForgotUsernameRequest from a JSON string
forgot_username_request_instance = ForgotUsernameRequest.from_json(json)
# print the JSON string representation of the object
print(ForgotUsernameRequest.to_json())

# convert the object into a dict
forgot_username_request_dict = forgot_username_request_instance.to_dict()
# create an instance of ForgotUsernameRequest from a dict
forgot_username_request_from_dict = ForgotUsernameRequest.from_dict(forgot_username_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


