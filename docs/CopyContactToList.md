# CopyContactToList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**Contact**](Contact.md) |  | [optional] 

## Example

```python
from clicksend.models.copy_contact_to_list import CopyContactToList

# TODO update the JSON string below
json = "{}"
# create an instance of CopyContactToList from a JSON string
copy_contact_to_list_instance = CopyContactToList.from_json(json)
# print the JSON string representation of the object
print(CopyContactToList.to_json())

# convert the object into a dict
copy_contact_to_list_dict = copy_contact_to_list_instance.to_dict()
# create an instance of CopyContactToList from a dict
copy_contact_to_list_from_dict = CopyContactToList.from_dict(copy_contact_to_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


