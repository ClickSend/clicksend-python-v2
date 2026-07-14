# AddAllowedEmailData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address_id** | **float** | The ID of the email address. | [optional] 
**email_address** | **str** | The email address. | [optional] 
**var_from** | **str** | The sender. | [optional] 

## Example

```python
from clicksend.models.add_allowed_email_data import AddAllowedEmailData

# TODO update the JSON string below
json = "{}"
# create an instance of AddAllowedEmailData from a JSON string
add_allowed_email_data_instance = AddAllowedEmailData.from_json(json)
# print the JSON string representation of the object
print(AddAllowedEmailData.to_json())

# convert the object into a dict
add_allowed_email_data_dict = add_allowed_email_data_instance.to_dict()
# create an instance of AddAllowedEmailData from a dict
add_allowed_email_data_from_dict = AddAllowedEmailData.from_dict(add_allowed_email_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


