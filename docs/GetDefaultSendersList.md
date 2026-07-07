# GetDefaultSendersList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | HTTP status code of the response. | 
**response_code** | **str** | Code indicating the result of the response. | 
**response_msg** | **str** | Message providing additional information. | 
**data** | [**GetDefaultSendersListData**](GetDefaultSendersListData.md) |  | 

## Example

```python
from clicksend.models.get_default_senders_list import GetDefaultSendersList

# TODO update the JSON string below
json = "{}"
# create an instance of GetDefaultSendersList from a JSON string
get_default_senders_list_instance = GetDefaultSendersList.from_json(json)
# print the JSON string representation of the object
print(GetDefaultSendersList.to_json())

# convert the object into a dict
get_default_senders_list_dict = get_default_senders_list_instance.to_dict()
# create an instance of GetDefaultSendersList from a dict
get_default_senders_list_from_dict = GetDefaultSendersList.from_dict(get_default_senders_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


