# ViewAvailableNumbersDataAllOfDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country** | **str** | The country code of the number. | [optional] 
**country_name** | **str** | The country name of the number. | [optional] 
**dedicated_number** | **str** | The dedicated number. | [optional] 
**price_setup** | **str** | The setup price of the number. | [optional] 
**price_monthly** | **str** | The monthly price of the number. | [optional] 
**price_total** | **str** | The total price of the number. | [optional] 
**address_requirement** | **str** | The address requirement for the number.  &lt;br&gt; &#x60;local&#x60;: requires an address that corresponds  to the phone number&#39;s prefix. | [optional] 

## Example

```python
from clicksend.models.view_available_numbers_data_all_of_data_inner import ViewAvailableNumbersDataAllOfDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAvailableNumbersDataAllOfDataInner from a JSON string
view_available_numbers_data_all_of_data_inner_instance = ViewAvailableNumbersDataAllOfDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewAvailableNumbersDataAllOfDataInner.to_json())

# convert the object into a dict
view_available_numbers_data_all_of_data_inner_dict = view_available_numbers_data_all_of_data_inner_instance.to_dict()
# create an instance of ViewAvailableNumbersDataAllOfDataInner from a dict
view_available_numbers_data_all_of_data_inner_from_dict = ViewAvailableNumbersDataAllOfDataInner.from_dict(view_available_numbers_data_all_of_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


