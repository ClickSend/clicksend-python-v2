# ViewListContacts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[Contact]**](Contact.md) |  | [optional] 

## Example

```python
from clicksend.models.view_list_contacts import ViewListContacts

# TODO update the JSON string below
json = "{}"
# create an instance of ViewListContacts from a JSON string
view_list_contacts_instance = ViewListContacts.from_json(json)
# print the JSON string representation of the object
print(ViewListContacts.to_json())

# convert the object into a dict
view_list_contacts_dict = view_list_contacts_instance.to_dict()
# create an instance of ViewListContacts from a dict
view_list_contacts_from_dict = ViewListContacts.from_dict(view_list_contacts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


