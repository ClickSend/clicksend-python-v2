# RemoveOptedOutContactsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**deleted** | **float** | The number of contacts deleted. | [optional] 

## Example

```python
from clicksend.models.remove_opted_out_contacts_data import RemoveOptedOutContactsData

# TODO update the JSON string below
json = "{}"
# create an instance of RemoveOptedOutContactsData from a JSON string
remove_opted_out_contacts_data_instance = RemoveOptedOutContactsData.from_json(json)
# print the JSON string representation of the object
print(RemoveOptedOutContactsData.to_json())

# convert the object into a dict
remove_opted_out_contacts_data_dict = remove_opted_out_contacts_data_instance.to_dict()
# create an instance of RemoveOptedOutContactsData from a dict
remove_opted_out_contacts_data_from_dict = RemoveOptedOutContactsData.from_dict(remove_opted_out_contacts_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


