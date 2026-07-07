# CalculateSmsCampaignPriceDataData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_from** | **str** | The sender. | [optional] 
**body** | **str** | The message body. | [optional] 
**schedule** | **str** | The schedule timestamp. | [optional] 

## Example

```python
from clicksend.models.calculate_sms_campaign_price_data_data import CalculateSmsCampaignPriceDataData

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateSmsCampaignPriceDataData from a JSON string
calculate_sms_campaign_price_data_data_instance = CalculateSmsCampaignPriceDataData.from_json(json)
# print the JSON string representation of the object
print(CalculateSmsCampaignPriceDataData.to_json())

# convert the object into a dict
calculate_sms_campaign_price_data_data_dict = calculate_sms_campaign_price_data_data_instance.to_dict()
# create an instance of CalculateSmsCampaignPriceDataData from a dict
calculate_sms_campaign_price_data_data_from_dict = CalculateSmsCampaignPriceDataData.from_dict(calculate_sms_campaign_price_data_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


