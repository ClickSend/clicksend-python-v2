# ViewYourNumbersDataAllOfDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dedicated_number** | **str** | The dedicated number. | [optional] 
**country** | **str** | The country. | [optional] 
**price** | **str** | The price. | [optional] 
**country_name** | **str** | The country name. | [optional] 
**notes** | **str** | Optional notes about the number. | [optional] 
**type** | **str** | The type of messages this number can send. | [optional] 
**number_type** | **str** | The classification of the number. | [optional] 
**number_category** | **str** | The category of the number. | [optional] 
**number_guid** | **str** | Unique identifier for the number. | [optional] 
**form_submission_id** | **str** | ID of any associated form submission. | [optional] 
**status** | [**ViewYourNumbersDataAllOfDataInnerStatus**](ViewYourNumbersDataAllOfDataInnerStatus.md) |  | [optional] 

## Example

```python
from clicksend.models.view_your_numbers_data_all_of_data_inner import ViewYourNumbersDataAllOfDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewYourNumbersDataAllOfDataInner from a JSON string
view_your_numbers_data_all_of_data_inner_instance = ViewYourNumbersDataAllOfDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewYourNumbersDataAllOfDataInner.to_json())

# convert the object into a dict
view_your_numbers_data_all_of_data_inner_dict = view_your_numbers_data_all_of_data_inner_instance.to_dict()
# create an instance of ViewYourNumbersDataAllOfDataInner from a dict
view_your_numbers_data_all_of_data_inner_from_dict = ViewYourNumbersDataAllOfDataInner.from_dict(view_your_numbers_data_all_of_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


