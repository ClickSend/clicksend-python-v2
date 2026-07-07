# CalculateMmsCampaignPriceDataData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_from** | **str** | The sender id. | [optional] 
**schedule** | **str** | The schedule timestamp. | [optional] 
**body** | **str** | The message body. | [optional] 

## Example

```python
from clicksend.models.calculate_mms_campaign_price_data_data import CalculateMmsCampaignPriceDataData

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateMmsCampaignPriceDataData from a JSON string
calculate_mms_campaign_price_data_data_instance = CalculateMmsCampaignPriceDataData.from_json(json)
# print the JSON string representation of the object
print(CalculateMmsCampaignPriceDataData.to_json())

# convert the object into a dict
calculate_mms_campaign_price_data_data_dict = calculate_mms_campaign_price_data_data_instance.to_dict()
# create an instance of CalculateMmsCampaignPriceDataData from a dict
calculate_mms_campaign_price_data_data_from_dict = CalculateMmsCampaignPriceDataData.from_dict(calculate_mms_campaign_price_data_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


