# ImportContacts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ImportContactsData**](ImportContactsData.md) |  | [optional] 

## Example

```python
from clicksend.models.import_contacts import ImportContacts

# TODO update the JSON string below
json = "{}"
# create an instance of ImportContacts from a JSON string
import_contacts_instance = ImportContacts.from_json(json)
# print the JSON string representation of the object
print(ImportContacts.to_json())

# convert the object into a dict
import_contacts_dict = import_contacts_instance.to_dict()
# create an instance of ImportContacts from a dict
import_contacts_from_dict = ImportContacts.from_dict(import_contacts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


