# RemoveDuplicateContacts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**RemoveOptedOutContactsData**](RemoveOptedOutContactsData.md) |  | [optional] 

## Example

```python
from clicksend.models.remove_duplicate_contacts import RemoveDuplicateContacts

# TODO update the JSON string below
json = "{}"
# create an instance of RemoveDuplicateContacts from a JSON string
remove_duplicate_contacts_instance = RemoveDuplicateContacts.from_json(json)
# print the JSON string representation of the object
print(RemoveDuplicateContacts.to_json())

# convert the object into a dict
remove_duplicate_contacts_dict = remove_duplicate_contacts_instance.to_dict()
# create an instance of RemoveDuplicateContacts from a dict
remove_duplicate_contacts_from_dict = RemoveDuplicateContacts.from_dict(remove_duplicate_contacts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


