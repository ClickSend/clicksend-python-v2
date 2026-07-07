# ListOwnNumbersMetadataPagination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_self** | **str** | The URL of the current page. | [optional] 
**next** | **str** | The URL of the next page. | [optional] 
**page_size** | **int** | The number of items returned per page. | [optional] 

## Example

```python
from clicksend.models.list_own_numbers_metadata_pagination import ListOwnNumbersMetadataPagination

# TODO update the JSON string below
json = "{}"
# create an instance of ListOwnNumbersMetadataPagination from a JSON string
list_own_numbers_metadata_pagination_instance = ListOwnNumbersMetadataPagination.from_json(json)
# print the JSON string representation of the object
print(ListOwnNumbersMetadataPagination.to_json())

# convert the object into a dict
list_own_numbers_metadata_pagination_dict = list_own_numbers_metadata_pagination_instance.to_dict()
# create an instance of ListOwnNumbersMetadataPagination from a dict
list_own_numbers_metadata_pagination_from_dict = ListOwnNumbersMetadataPagination.from_dict(list_own_numbers_metadata_pagination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


