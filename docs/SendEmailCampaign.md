# SendEmailCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SendEmailCampaignData**](SendEmailCampaignData.md) |  | [optional] 

## Example

```python
from clicksend.models.send_email_campaign import SendEmailCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailCampaign from a JSON string
send_email_campaign_instance = SendEmailCampaign.from_json(json)
# print the JSON string representation of the object
print(SendEmailCampaign.to_json())

# convert the object into a dict
send_email_campaign_dict = send_email_campaign_instance.to_dict()
# create an instance of SendEmailCampaign from a dict
send_email_campaign_from_dict = SendEmailCampaign.from_dict(send_email_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


