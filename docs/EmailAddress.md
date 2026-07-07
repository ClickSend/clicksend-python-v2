# EmailAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address_id** | **int** | The unique identifier for the email address. | [optional] 
**email_address** | **str** | The email address. | [optional] 
**verified** | **int** | Flag indicating if the email address is verified. | [optional] 
**date_added** | **str** | The date the email address was added. | [optional] 

## Example

```python
from clicksend.models.email_address import EmailAddress

# TODO update the JSON string below
json = "{}"
# create an instance of EmailAddress from a JSON string
email_address_instance = EmailAddress.from_json(json)
# print the JSON string representation of the object
print(EmailAddress.to_json())

# convert the object into a dict
email_address_dict = email_address_instance.to_dict()
# create an instance of EmailAddress from a dict
email_address_from_dict = EmailAddress.from_dict(email_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


