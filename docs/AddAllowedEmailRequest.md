# AddAllowedEmailRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**from_fax** | **str** |  | [optional] 
**subaccount_id** | **str** |  | [optional] 

## Example

```python
from clicksend.models.add_allowed_email_request import AddAllowedEmailRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AddAllowedEmailRequest from a JSON string
add_allowed_email_request_instance = AddAllowedEmailRequest.from_json(json)
# print the JSON string representation of the object
print(AddAllowedEmailRequest.to_json())

# convert the object into a dict
add_allowed_email_request_dict = add_allowed_email_request_instance.to_dict()
# create an instance of AddAllowedEmailRequest from a dict
add_allowed_email_request_from_dict = AddAllowedEmailRequest.from_dict(add_allowed_email_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


