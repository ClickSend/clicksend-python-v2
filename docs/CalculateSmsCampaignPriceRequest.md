# CalculateSmsCampaignPriceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**list_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateSmsCampaignPriceRequest from a JSON string
calculate_sms_campaign_price_request_instance = CalculateSmsCampaignPriceRequest.from_json(json)
# print the JSON string representation of the object
print(CalculateSmsCampaignPriceRequest.to_json())

# convert the object into a dict
calculate_sms_campaign_price_request_dict = calculate_sms_campaign_price_request_instance.to_dict()
# create an instance of CalculateSmsCampaignPriceRequest from a dict
calculate_sms_campaign_price_request_from_dict = CalculateSmsCampaignPriceRequest.from_dict(calculate_sms_campaign_price_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


