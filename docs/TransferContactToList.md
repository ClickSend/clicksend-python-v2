# TransferContactToList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**Contact**](Contact.md) |  | [optional] 

## Example

```python
from clicksend.models.transfer_contact_to_list import TransferContactToList

# TODO update the JSON string below
json = "{}"
# create an instance of TransferContactToList from a JSON string
transfer_contact_to_list_instance = TransferContactToList.from_json(json)
# print the JSON string representation of the object
print(TransferContactToList.to_json())

# convert the object into a dict
transfer_contact_to_list_dict = transfer_contact_to_list_instance.to_dict()
# create an instance of TransferContactToList from a dict
transfer_contact_to_list_from_dict = TransferContactToList.from_dict(transfer_contact_to_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


