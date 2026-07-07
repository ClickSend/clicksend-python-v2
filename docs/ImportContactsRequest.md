# ImportContactsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_url** | **str** |  | [optional] 
**field_order** | **str** |  | [optional] 

## Example

```python
from clicksend.models.import_contacts_request import ImportContactsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ImportContactsRequest from a JSON string
import_contacts_request_instance = ImportContactsRequest.from_json(json)
# print the JSON string representation of the object
print(ImportContactsRequest.to_json())

# convert the object into a dict
import_contacts_request_dict = import_contacts_request_instance.to_dict()
# create an instance of ImportContactsRequest from a dict
import_contacts_request_from_dict = ImportContactsRequest.from_dict(import_contacts_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


