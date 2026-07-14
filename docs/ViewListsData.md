# ViewListsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** | The total number of contacts in the list. | [optional] 
**per_page** | **int** | The number of contacts returned per page. | [optional] 
**current_page** | **int** | The current page number. | [optional] 
**last_page** | **int** | The total number of pages. | [optional] 
**next_page_url** | **str** | The URL of the next page of contacts. | [optional] 
**prev_page_url** | **str** | The URL of the previous page of contacts. | [optional] 
**var_from** | **int** | The number of the first contact on the current page. | [optional] 
**to** | **int** | The number of the last contact on the current page. | [optional] 
**first_page_url** | **str** | The URL of the first page of records. | [optional] 
**last_page_url** | **str** | The URL of the last page of records. | [optional] 
**path** | **str** | The base URL path used to build pagination links. | [optional] 
**links** | [**List[ViewListsDataLinksInner]**](ViewListsDataLinksInner.md) | The list of pagination links. | [optional] 
**data** | [**List[ContactList]**](ContactList.md) | The contacts in the list. | [optional] 

## Example

```python
from clicksend.models.view_lists_data import ViewListsData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewListsData from a JSON string
view_lists_data_instance = ViewListsData.from_json(json)
# print the JSON string representation of the object
print(ViewListsData.to_json())

# convert the object into a dict
view_lists_data_dict = view_lists_data_instance.to_dict()
# create an instance of ViewListsData from a dict
view_lists_data_from_dict = ViewListsData.from_dict(view_lists_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


