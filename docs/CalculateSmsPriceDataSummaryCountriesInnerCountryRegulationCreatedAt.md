# CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt

The parameters related to the time of your request.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **datetime** | The time you made the request. It will be in &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/ISO_8601\&quot; target&#x3D;\&quot;_blank\&quot;&gt;ISO 8601&lt;/a&gt; format. | [optional] 
**timezone_type** | **int** | The offset value from the time you made the request. | [optional] 
**timezone** | **str** | The timezone when you made the request. | [optional] 

## Example

```python
from clicksend.models.calculate_sms_price_data_summary_countries_inner_country_regulation_created_at import CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt from a JSON string
calculate_sms_price_data_summary_countries_inner_country_regulation_created_at_instance = CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt.from_json(json)
# print the JSON string representation of the object
print(CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt.to_json())

# convert the object into a dict
calculate_sms_price_data_summary_countries_inner_country_regulation_created_at_dict = calculate_sms_price_data_summary_countries_inner_country_regulation_created_at_instance.to_dict()
# create an instance of CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt from a dict
calculate_sms_price_data_summary_countries_inner_country_regulation_created_at_from_dict = CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt.from_dict(calculate_sms_price_data_summary_countries_inner_country_regulation_created_at_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


