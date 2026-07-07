# ImportContactsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**msg** | **str** | The message to display. | [optional] 
**ids** | **List[str]** | The list of ids of the imported contacts. | [optional] 
**id** | **str** | The list id of the imported contacts. | [optional] 

## Example

```python
from clicksend.models.import_contacts_data import ImportContactsData

# TODO update the JSON string below
json = "{}"
# create an instance of ImportContactsData from a JSON string
import_contacts_data_instance = ImportContactsData.from_json(json)
# print the JSON string representation of the object
print(ImportContactsData.to_json())

# convert the object into a dict
import_contacts_data_dict = import_contacts_data_instance.to_dict()
# create an instance of ImportContactsData from a dict
import_contacts_data_from_dict = ImportContactsData.from_dict(import_contacts_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


