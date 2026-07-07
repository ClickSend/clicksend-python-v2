# SelectCountriesForGlobalSendingRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country_list_ids** | **List[int]** |  | [optional] 

## Example

```python
from clicksend.models.select_countries_for_global_sending_request import SelectCountriesForGlobalSendingRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SelectCountriesForGlobalSendingRequest from a JSON string
select_countries_for_global_sending_request_instance = SelectCountriesForGlobalSendingRequest.from_json(json)
# print the JSON string representation of the object
print(SelectCountriesForGlobalSendingRequest.to_json())

# convert the object into a dict
select_countries_for_global_sending_request_dict = select_countries_for_global_sending_request_instance.to_dict()
# create an instance of SelectCountriesForGlobalSendingRequest from a dict
select_countries_for_global_sending_request_from_dict = SelectCountriesForGlobalSendingRequest.from_dict(select_countries_for_global_sending_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


