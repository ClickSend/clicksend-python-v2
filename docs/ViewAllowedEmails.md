# ViewAllowedEmails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[ViewAllowedEmailsDataInner]**](ViewAllowedEmailsDataInner.md) |  | [optional] 

## Example

```python
from clicksend.models.view_allowed_emails import ViewAllowedEmails

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAllowedEmails from a JSON string
view_allowed_emails_instance = ViewAllowedEmails.from_json(json)
# print the JSON string representation of the object
print(ViewAllowedEmails.to_json())

# convert the object into a dict
view_allowed_emails_dict = view_allowed_emails_instance.to_dict()
# create an instance of ViewAllowedEmails from a dict
view_allowed_emails_from_dict = ViewAllowedEmails.from_dict(view_allowed_emails_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


