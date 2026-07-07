# CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation

The parameters related to the country guidelines on the user level.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country_user_id** | **int** | Your identifier for the country regulation. | [optional] 
**sms_registration_type** | **int** | The global sending requirement for this country. It can be one of the following:  - **0:** No number or account registration required.      - **1:** Number registration required. You can purchase a registered number from ClickSend. Examples: US and CA.      - **2:** Account registration required. You can register your company details or business details to register your account. Examples: NZ, SG and UAE.  This parameter is a duplicate of registration_type.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This parameter is fixed and can&#39;t be changed based on your settings.&lt;/p&gt; &lt;/div&gt; | [optional] 
**restricted_sending** | **bool** | Indicates whether you have any restriction for sending the message to this country:  - **True:** You&#39;re restricted from sending messages to this country, possibly due to not having a registered number.      - **False:** You&#39;re not restricted from sending messages to this country. | [optional] 
**trial_sending** | **bool** | Indicates whether the country supports trial sending or not:  - **True:** This country supports trial sending      - **False:** This country doesn’t support trial sending  Countries with restricted sending typically offers trial sending. With trial sending, you can send messages to the country without registering your number or account.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;Trial sending has limitations, such as a daily limit of 200 messages in some countries. The limitations vary by country. &lt;br/&gt;&lt;br/&gt; This parameter is fixed and can&#39;t be changed based on your settings.&lt;/p&gt; &lt;/div&gt; | [optional] 
**regulation_requirements_description** | **str** | The text description of the regulatory requirements. | [optional] 
**created_at** | [**CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt**](CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt.md) |  | [optional] 
**updated_at** | [**CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt**](CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_sms_price_data_summary_countries_inner_country_regulation import CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation from a JSON string
calculate_sms_price_data_summary_countries_inner_country_regulation_instance = CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation.from_json(json)
# print the JSON string representation of the object
print(CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation.to_json())

# convert the object into a dict
calculate_sms_price_data_summary_countries_inner_country_regulation_dict = calculate_sms_price_data_summary_countries_inner_country_regulation_instance.to_dict()
# create an instance of CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation from a dict
calculate_sms_price_data_summary_countries_inner_country_regulation_from_dict = CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation.from_dict(calculate_sms_price_data_summary_countries_inner_country_regulation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


