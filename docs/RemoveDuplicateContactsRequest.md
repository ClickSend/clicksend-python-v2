# RemoveDuplicateContactsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fields** | [**RemoveDuplicateContactsRequestFields**](RemoveDuplicateContactsRequestFields.md) |  | [optional] 

## Example

```python
from clicksend.models.remove_duplicate_contacts_request import RemoveDuplicateContactsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RemoveDuplicateContactsRequest from a JSON string
remove_duplicate_contacts_request_instance = RemoveDuplicateContactsRequest.from_json(json)
# print the JSON string representation of the object
print(RemoveDuplicateContactsRequest.to_json())

# convert the object into a dict
remove_duplicate_contacts_request_dict = remove_duplicate_contacts_request_instance.to_dict()
# create an instance of RemoveDuplicateContactsRequest from a dict
remove_duplicate_contacts_request_from_dict = RemoveDuplicateContactsRequest.from_dict(remove_duplicate_contacts_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


