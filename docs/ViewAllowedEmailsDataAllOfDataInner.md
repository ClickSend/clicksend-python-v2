# ViewAllowedEmailsDataAllOfDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address_id** | **float** | The ID of the email address. | [optional] 
**email_address** | **str** | The email address. | [optional] 
**var_from** | **str** | The sender. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount that owns this email address. | [optional] 
**from_fax** | **str** | The fax number used as the sender, if applicable. | [optional] 
**voice** | **str** | The voice used when this email address triggers a voice message. | [optional] 
**lang** | **str** | The language used when this email address triggers a voice message. | [optional] 
**subaccount_name** | **str** | The name of the subaccount that owns this email address. | [optional] 

## Example

```python
from clicksend.models.view_allowed_emails_data_all_of_data_inner import ViewAllowedEmailsDataAllOfDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAllowedEmailsDataAllOfDataInner from a JSON string
view_allowed_emails_data_all_of_data_inner_instance = ViewAllowedEmailsDataAllOfDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewAllowedEmailsDataAllOfDataInner.to_json())

# convert the object into a dict
view_allowed_emails_data_all_of_data_inner_dict = view_allowed_emails_data_all_of_data_inner_instance.to_dict()
# create an instance of ViewAllowedEmailsDataAllOfDataInner from a dict
view_allowed_emails_data_all_of_data_inner_from_dict = ViewAllowedEmailsDataAllOfDataInner.from_dict(view_allowed_emails_data_all_of_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


