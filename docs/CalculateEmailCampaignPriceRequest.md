# CalculateEmailCampaignPriceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**from_email_address_id** | **str** |  | [optional] 
**template_id** | **str** |  | [optional] 
**list_id** | **str** |  | [optional] 
**from_name** | **str** |  | [optional] 
**draft** | **int** |  | [optional] 
**schedule** | **str** |  | [optional] 
**custom_string** | **str** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from clicksend.models.calculate_email_campaign_price_request import CalculateEmailCampaignPriceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateEmailCampaignPriceRequest from a JSON string
calculate_email_campaign_price_request_instance = CalculateEmailCampaignPriceRequest.from_json(json)
# print the JSON string representation of the object
print(CalculateEmailCampaignPriceRequest.to_json())

# convert the object into a dict
calculate_email_campaign_price_request_dict = calculate_email_campaign_price_request_instance.to_dict()
# create an instance of CalculateEmailCampaignPriceRequest from a dict
calculate_email_campaign_price_request_from_dict = CalculateEmailCampaignPriceRequest.from_dict(calculate_email_campaign_price_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


