# ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_global** | **bool** | Whether this sender type is allowed sending from any country | 
**country_codes** | **List[str]** | List of ISO 3166-1 alpha-2 formatted country codes | [optional] 

## Example

```python
from clicksend.models.list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_allowed_sender_countries import ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries

# TODO update the JSON string below
json = "{}"
# create an instance of ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries from a JSON string
list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_allowed_sender_countries_instance = ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries.from_json(json)
# print the JSON string representation of the object
print(ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries.to_json())

# convert the object into a dict
list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_allowed_sender_countries_dict = list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_allowed_sender_countries_instance.to_dict()
# create an instance of ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries from a dict
list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_allowed_sender_countries_from_dict = ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInnerAllowedSenderCountries.from_dict(list_compliant_sender_types200_response_data_data_inner_allowed_sender_types_inner_allowed_sender_countries_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


