# ViewAllowedEmailsDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address_id** | **float** | The ID of the email address. | [optional] 
**email_address** | **str** | The email address. | [optional] 
**var_from** | **str** | The sender. | [optional] 

## Example

```python
from clicksend.models.view_allowed_emails_data_inner import ViewAllowedEmailsDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAllowedEmailsDataInner from a JSON string
view_allowed_emails_data_inner_instance = ViewAllowedEmailsDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewAllowedEmailsDataInner.to_json())

# convert the object into a dict
view_allowed_emails_data_inner_dict = view_allowed_emails_data_inner_instance.to_dict()
# create an instance of ViewAllowedEmailsDataInner from a dict
view_allowed_emails_data_inner_from_dict = ViewAllowedEmailsDataInner.from_dict(view_allowed_emails_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


