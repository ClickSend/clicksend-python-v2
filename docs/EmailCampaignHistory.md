# EmailCampaignHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_campaign_id** | **int** | The ID of the email campaign. | [optional] 
**from_name** | **str** | The name of the sender. | [optional] 
**from_address** | **str** | The email address of the sender. | [optional] 
**to_name** | **str** | The name of the recipient. | [optional] 
**to_address** | **str** | The email address of the recipient. | [optional] 
**contact_id** | **int** | The ID of the contact associated with the email. | [optional] 
**subject** | **str** | The subject of the email. | [optional] 
**message_id** | **str** | The unique ID of the email message. | [optional] 
**processed_at** | **str** | The date and time when the email was processed. | [optional] 
**status** | **str** | The status of the email (e.g., SpamReport, Sent). | [optional] 
**open_count** | **int** | The count of times the email was opened. | [optional] 
**click_count** | **int** | The count of times links in the email were clicked. | [optional] 
**hard_bounce_count** | **int** | The count of hard bounces for the email. | [optional] 
**soft_bounce_count** | **int** | The count of soft bounces for the email. | [optional] 

## Example

```python
from clicksend.models.email_campaign_history import EmailCampaignHistory

# TODO update the JSON string below
json = "{}"
# create an instance of EmailCampaignHistory from a JSON string
email_campaign_history_instance = EmailCampaignHistory.from_json(json)
# print the JSON string representation of the object
print(EmailCampaignHistory.to_json())

# convert the object into a dict
email_campaign_history_dict = email_campaign_history_instance.to_dict()
# create an instance of EmailCampaignHistory from a dict
email_campaign_history_from_dict = EmailCampaignHistory.from_dict(email_campaign_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


