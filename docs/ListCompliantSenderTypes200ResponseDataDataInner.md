# ListCompliantSenderTypes200ResponseDataDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipient_country_code** | **str** | ISO 3166-1 alpha-2 formatted country code | 
**blocked_sender_types** | **List[str]** | List of blocked sender types in recipient country | 
**allowed_sender_types** | [**List[ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner]**](ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner.md) |  | 

## Example

```python
from clicksend.models.list_compliant_sender_types200_response_data_data_inner import ListCompliantSenderTypes200ResponseDataDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCompliantSenderTypes200ResponseDataDataInner from a JSON string
list_compliant_sender_types200_response_data_data_inner_instance = ListCompliantSenderTypes200ResponseDataDataInner.from_json(json)
# print the JSON string representation of the object
print(ListCompliantSenderTypes200ResponseDataDataInner.to_json())

# convert the object into a dict
list_compliant_sender_types200_response_data_data_inner_dict = list_compliant_sender_types200_response_data_data_inner_instance.to_dict()
# create an instance of ListCompliantSenderTypes200ResponseDataDataInner from a dict
list_compliant_sender_types200_response_data_data_inner_from_dict = ListCompliantSenderTypes200ResponseDataDataInner.from_dict(list_compliant_sender_types200_response_data_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


