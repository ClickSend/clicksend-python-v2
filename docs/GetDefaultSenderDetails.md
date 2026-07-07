# GetDefaultSenderDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | HTTP status code of the response. | 
**response_code** | **str** | Code indicating the result of the response. | 
**response_msg** | **str** | Message providing additional information. | 
**data** | [**DefaultSender**](DefaultSender.md) |  | 

## Example

```python
from clicksend.models.get_default_sender_details import GetDefaultSenderDetails

# TODO update the JSON string below
json = "{}"
# create an instance of GetDefaultSenderDetails from a JSON string
get_default_sender_details_instance = GetDefaultSenderDetails.from_json(json)
# print the JSON string representation of the object
print(GetDefaultSenderDetails.to_json())

# convert the object into a dict
get_default_sender_details_dict = get_default_sender_details_instance.to_dict()
# create an instance of GetDefaultSenderDetails from a dict
get_default_sender_details_from_dict = GetDefaultSenderDetails.from_dict(get_default_sender_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


