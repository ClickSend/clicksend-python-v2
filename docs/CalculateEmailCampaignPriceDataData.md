# CalculateEmailCampaignPriceDataData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Name. | [optional] 
**subject** | **str** | Your template subject. | [optional] 
**from_email_address_id** | **float** | The allowed email address id. | [optional] 
**from_name** | **str** | Your sender name. | [optional] 
**body** | **str** | Your message. | [optional] 
**list_id** | **float** | Your list id. | [optional] 

## Example

```python
from clicksend.models.calculate_email_campaign_price_data_data import CalculateEmailCampaignPriceDataData

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateEmailCampaignPriceDataData from a JSON string
calculate_email_campaign_price_data_data_instance = CalculateEmailCampaignPriceDataData.from_json(json)
# print the JSON string representation of the object
print(CalculateEmailCampaignPriceDataData.to_json())

# convert the object into a dict
calculate_email_campaign_price_data_data_dict = calculate_email_campaign_price_data_data_instance.to_dict()
# create an instance of CalculateEmailCampaignPriceDataData from a dict
calculate_email_campaign_price_data_data_from_dict = CalculateEmailCampaignPriceDataData.from_dict(calculate_email_campaign_price_data_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


