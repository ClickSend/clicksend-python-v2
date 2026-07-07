# CreateNewContact


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**Contact**](Contact.md) |  | [optional] 

## Example

```python
from clicksend.models.create_new_contact import CreateNewContact

# TODO update the JSON string below
json = "{}"
# create an instance of CreateNewContact from a JSON string
create_new_contact_instance = CreateNewContact.from_json(json)
# print the JSON string representation of the object
print(CreateNewContact.to_json())

# convert the object into a dict
create_new_contact_dict = create_new_contact_instance.to_dict()
# create an instance of CreateNewContact from a dict
create_new_contact_from_dict = CreateNewContact.from_dict(create_new_contact_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


