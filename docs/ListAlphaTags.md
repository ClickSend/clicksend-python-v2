# ListAlphaTags


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alpha_tags** | [**List[AlphaTag]**](AlphaTag.md) | The list of alpha tags. | [optional] 
**metadata** | [**ListOwnNumbersMetadata**](ListOwnNumbersMetadata.md) |  | [optional] 

## Example

```python
from clicksend.models.list_alpha_tags import ListAlphaTags

# TODO update the JSON string below
json = "{}"
# create an instance of ListAlphaTags from a JSON string
list_alpha_tags_instance = ListAlphaTags.from_json(json)
# print the JSON string representation of the object
print(ListAlphaTags.to_json())

# convert the object into a dict
list_alpha_tags_dict = list_alpha_tags_instance.to_dict()
# create an instance of ListAlphaTags from a dict
list_alpha_tags_from_dict = ListAlphaTags.from_dict(list_alpha_tags_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


