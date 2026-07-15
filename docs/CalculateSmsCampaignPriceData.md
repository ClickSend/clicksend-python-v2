# CalculateSmsCampaignPriceData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_count** | **int** | The total number of records. | [optional] 
**total_price** | **str** | The total price of the SMS campaign. | [optional] 
**data** | [**CalculateSmsCampaignPriceDataData**](CalculateSmsCampaignPriceDataData.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_sms_campaign_price_data import CalculateSmsCampaignPriceData

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateSmsCampaignPriceData from a JSON string
calculate_sms_campaign_price_data_instance = CalculateSmsCampaignPriceData.from_json(json)
# print the JSON string representation of the object
print(CalculateSmsCampaignPriceData.to_json())

# convert the object into a dict
calculate_sms_campaign_price_data_dict = calculate_sms_campaign_price_data_instance.to_dict()
# create an instance of CalculateSmsCampaignPriceData from a dict
calculate_sms_campaign_price_data_from_dict = CalculateSmsCampaignPriceData.from_dict(calculate_sms_campaign_price_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


