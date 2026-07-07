# CreateAllowedEmailAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**EmailAddress**](EmailAddress.md) |  | [optional] 

## Example

```python
from clicksend.models.create_allowed_email_address import CreateAllowedEmailAddress

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAllowedEmailAddress from a JSON string
create_allowed_email_address_instance = CreateAllowedEmailAddress.from_json(json)
# print the JSON string representation of the object
print(CreateAllowedEmailAddress.to_json())

# convert the object into a dict
create_allowed_email_address_dict = create_allowed_email_address_instance.to_dict()
# create an instance of CreateAllowedEmailAddress from a dict
create_allowed_email_address_from_dict = CreateAllowedEmailAddress.from_dict(create_allowed_email_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


