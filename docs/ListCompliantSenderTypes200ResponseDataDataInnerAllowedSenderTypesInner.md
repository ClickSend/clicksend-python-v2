# ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sender_type** | **str** | Type of sender | 
**allowed_sender_countries** | [**ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries**](ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries.md) |  | 

## Example

```python
from clicksend.models.list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner import ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner from a JSON string
list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_instance = ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner.from_json(json)
# print the JSON string representation of the object
print(ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner.to_json())

# convert the object into a dict
list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_dict = list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_instance.to_dict()
# create an instance of ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner from a dict
list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_from_dict = ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner.from_dict(list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


