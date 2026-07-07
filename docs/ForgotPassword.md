# ForgotPassword


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **List[str]** |  | [optional] 

## Example

```python
from clicksend.models.forgot_password import ForgotPassword

# TODO update the JSON string below
json = "{}"
# create an instance of ForgotPassword from a JSON string
forgot_password_instance = ForgotPassword.from_json(json)
# print the JSON string representation of the object
print(ForgotPassword.to_json())

# convert the object into a dict
forgot_password_dict = forgot_password_instance.to_dict()
# create an instance of ForgotPassword from a dict
forgot_password_from_dict = ForgotPassword.from_dict(forgot_password_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


