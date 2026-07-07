# CalculateEmailCampaignPriceData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_count** | **float** | The total count of the email campaigns. | [optional] 
**total_price** | **str** | The total price of the email campaigns. | [optional] 
**queued_count** | **float** | The count of the queued email campaigns. | [optional] 
**data** | [**CalculateEmailCampaignPriceDataData**](CalculateEmailCampaignPriceDataData.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_email_campaign_price_data import CalculateEmailCampaignPriceData

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateEmailCampaignPriceData from a JSON string
calculate_email_campaign_price_data_instance = CalculateEmailCampaignPriceData.from_json(json)
# print the JSON string representation of the object
print(CalculateEmailCampaignPriceData.to_json())

# convert the object into a dict
calculate_email_campaign_price_data_dict = calculate_email_campaign_price_data_instance.to_dict()
# create an instance of CalculateEmailCampaignPriceData from a dict
calculate_email_campaign_price_data_from_dict = CalculateEmailCampaignPriceData.from_dict(calculate_email_campaign_price_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


