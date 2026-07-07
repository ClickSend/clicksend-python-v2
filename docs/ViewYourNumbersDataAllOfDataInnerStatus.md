# ViewYourNumbersDataAllOfDataInnerStatus

The registration status of the number.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **int** | Numeric status code (0-5): - 0: Your number is ready to go. - 1: Your number is unregistered. You will not be able to send messages to certain countries. - 2: Your number registration is in progress. Email updates will follow. - 3: Action required on your number registration. Please resolve to start using it. - 4: You can send to all countries but may get restricted to some before full registration. - 5: Your number is registered and you can start using it immediately.  | [optional] 
**label** | **str** | Status label identifier corresponding to the numeric value above, following the same order. | [optional] 
**description** | **str** | Human readable description of the status. | [optional] 
**name** | **str** | Display name for the status corresponding to the numeric value above, following the same order. | [optional] 

## Example

```python
from clicksend.models.view_your_numbers_data_all_of_data_inner_status import ViewYourNumbersDataAllOfDataInnerStatus

# TODO update the JSON string below
json = "{}"
# create an instance of ViewYourNumbersDataAllOfDataInnerStatus from a JSON string
view_your_numbers_data_all_of_data_inner_status_instance = ViewYourNumbersDataAllOfDataInnerStatus.from_json(json)
# print the JSON string representation of the object
print(ViewYourNumbersDataAllOfDataInnerStatus.to_json())

# convert the object into a dict
view_your_numbers_data_all_of_data_inner_status_dict = view_your_numbers_data_all_of_data_inner_status_instance.to_dict()
# create an instance of ViewYourNumbersDataAllOfDataInnerStatus from a dict
view_your_numbers_data_all_of_data_inner_status_from_dict = ViewYourNumbersDataAllOfDataInnerStatus.from_dict(view_your_numbers_data_all_of_data_inner_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


