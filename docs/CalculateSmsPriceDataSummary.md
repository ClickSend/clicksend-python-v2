# CalculateSmsPriceDataSummary

The parameters for additional summary. It shows the guidelines for each country you have selected.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**test_message** | **str** | This parameter is used for internal developers. This is used when your account is in trial period. | [optional] 
**countries** | [**List[CalculateSmsPriceDataSummaryCountriesInner]**](CalculateSmsPriceDataSummaryCountriesInner.md) | The list of countries of the receipients in two-letter format (e.g. US, UK, AU, NZ, etc). | [optional] 

## Example

```python
from clicksend.models.calculate_sms_price_data_summary import CalculateSmsPriceDataSummary

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateSmsPriceDataSummary from a JSON string
calculate_sms_price_data_summary_instance = CalculateSmsPriceDataSummary.from_json(json)
# print the JSON string representation of the object
print(CalculateSmsPriceDataSummary.to_json())

# convert the object into a dict
calculate_sms_price_data_summary_dict = calculate_sms_price_data_summary_instance.to_dict()
# create an instance of CalculateSmsPriceDataSummary from a dict
calculate_sms_price_data_summary_from_dict = CalculateSmsPriceDataSummary.from_dict(calculate_sms_price_data_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


