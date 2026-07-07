# SendEmailCampaignData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**totlal_count** | **float** | The total count of the email campaigns. | [optional] 
**total_price** | **str** | The total price of the email campaigns. | [optional] 
**queued_count** | **float** | The count of the queued email campaigns. | [optional] 
**data** | [**EmailCampaign**](EmailCampaign.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.send_email_campaign_data import SendEmailCampaignData

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailCampaignData from a JSON string
send_email_campaign_data_instance = SendEmailCampaignData.from_json(json)
# print the JSON string representation of the object
print(SendEmailCampaignData.to_json())

# convert the object into a dict
send_email_campaign_data_dict = send_email_campaign_data_instance.to_dict()
# create an instance of SendEmailCampaignData from a dict
send_email_campaign_data_from_dict = SendEmailCampaignData.from_dict(send_email_campaign_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


