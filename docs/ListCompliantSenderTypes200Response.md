# ListCompliantSenderTypes200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | HTTP status code of the response | 
**response_code** | **str** | Code indicating the result of the response | 
**response_msg** | **str** | Message providing additional information | 
**data** | [**ListCompliantSenderTypes200ResponseData**](ListCompliantSenderTypes200ResponseData.md) |  | 

## Example

```python
from clicksend.models.list_compliant_sender_types200_response import ListCompliantSenderTypes200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListCompliantSenderTypes200Response from a JSON string
list_compliant_sender_types200_response_instance = ListCompliantSenderTypes200Response.from_json(json)
# print the JSON string representation of the object
print(ListCompliantSenderTypes200Response.to_json())

# convert the object into a dict
list_compliant_sender_types200_response_dict = list_compliant_sender_types200_response_instance.to_dict()
# create an instance of ListCompliantSenderTypes200Response from a dict
list_compliant_sender_types200_response_from_dict = ListCompliantSenderTypes200Response.from_dict(list_compliant_sender_types200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


