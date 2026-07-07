# GetDefaultSendersListData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[DefaultSender]**](DefaultSender.md) | List of default senders. | [optional] 
**per_page** | **int** | Number of items per page. | [optional] 
**self_page_url** | **str** | URL for the current page. | [optional] 
**next_page_url** | **str** | URL for the next page. | [optional] 

## Example

```python
from clicksend.models.get_default_senders_list_data import GetDefaultSendersListData

# TODO update the JSON string below
json = "{}"
# create an instance of GetDefaultSendersListData from a JSON string
get_default_senders_list_data_instance = GetDefaultSendersListData.from_json(json)
# print the JSON string representation of the object
print(GetDefaultSendersListData.to_json())

# convert the object into a dict
get_default_senders_list_data_dict = get_default_senders_list_data_instance.to_dict()
# create an instance of GetDefaultSendersListData from a dict
get_default_senders_list_data_from_dict = GetDefaultSendersListData.from_dict(get_default_senders_list_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


