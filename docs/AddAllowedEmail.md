# AddAllowedEmail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**AddAllowedEmailData**](AddAllowedEmailData.md) |  | [optional] 

## Example

```python
from clicksend.models.add_allowed_email import AddAllowedEmail

# TODO update the JSON string below
json = "{}"
# create an instance of AddAllowedEmail from a JSON string
add_allowed_email_instance = AddAllowedEmail.from_json(json)
# print the JSON string representation of the object
print(AddAllowedEmail.to_json())

# convert the object into a dict
add_allowed_email_dict = add_allowed_email_instance.to_dict()
# create an instance of AddAllowedEmail from a dict
add_allowed_email_from_dict = AddAllowedEmail.from_dict(add_allowed_email_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


