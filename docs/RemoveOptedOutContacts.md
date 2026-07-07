# RemoveOptedOutContacts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**RemoveOptedOutContactsData**](RemoveOptedOutContactsData.md) |  | [optional] 

## Example

```python
from clicksend.models.remove_opted_out_contacts import RemoveOptedOutContacts

# TODO update the JSON string below
json = "{}"
# create an instance of RemoveOptedOutContacts from a JSON string
remove_opted_out_contacts_instance = RemoveOptedOutContacts.from_json(json)
# print the JSON string representation of the object
print(RemoveOptedOutContacts.to_json())

# convert the object into a dict
remove_opted_out_contacts_dict = remove_opted_out_contacts_instance.to_dict()
# create an instance of RemoveOptedOutContacts from a dict
remove_opted_out_contacts_from_dict = RemoveOptedOutContacts.from_dict(remove_opted_out_contacts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


