# RemoveDuplicateContactsRequestFields


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.remove_duplicate_contacts_request_fields import RemoveDuplicateContactsRequestFields

# TODO update the JSON string below
json = "{}"
# create an instance of RemoveDuplicateContactsRequestFields from a JSON string
remove_duplicate_contacts_request_fields_instance = RemoveDuplicateContactsRequestFields.from_json(json)
# print the JSON string representation of the object
print(RemoveDuplicateContactsRequestFields.to_json())

# convert the object into a dict
remove_duplicate_contacts_request_fields_dict = remove_duplicate_contacts_request_fields_instance.to_dict()
# create an instance of RemoveDuplicateContactsRequestFields from a dict
remove_duplicate_contacts_request_fields_from_dict = RemoveDuplicateContactsRequestFields.from_dict(remove_duplicate_contacts_request_fields_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


