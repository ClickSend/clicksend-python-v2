# ListOwnNumbers


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**own_numbers** | [**List[OwnNumber]**](OwnNumber.md) | The list of own numbers. | [optional] 
**metadata** | [**ListOwnNumbersMetadata**](ListOwnNumbersMetadata.md) |  | [optional] 

## Example

```python
from clicksend.models.list_own_numbers import ListOwnNumbers

# TODO update the JSON string below
json = "{}"
# create an instance of ListOwnNumbers from a JSON string
list_own_numbers_instance = ListOwnNumbers.from_json(json)
# print the JSON string representation of the object
print(ListOwnNumbers.to_json())

# convert the object into a dict
list_own_numbers_dict = list_own_numbers_instance.to_dict()
# create an instance of ListOwnNumbers from a dict
list_own_numbers_from_dict = ListOwnNumbers.from_dict(list_own_numbers_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


