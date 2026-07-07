# EmailCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_campaign_id** | **int** | The ID of the email campaign. | [optional] 
**name** | **str** | The name of the email campaign. | [optional] 
**user_id** | **int** | The ID of the user who created the email campaign. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount associated with the email campaign. | [optional] 
**subject** | **str** | The subject of the email campaign. | [optional] 
**list_id** | **int** | The ID of the email list associated with the campaign. | [optional] 
**from_email_address_id** | **int** | The ID of the sender&#39;s email address. | [optional] 
**from_name** | **str** | The name of the sender. | [optional] 
**template_id** | **int** | The ID of the email template used in the campaign. | [optional] 
**schedule** | **str** | The schedule for sending the email campaign. | [optional] 
**status** | **str** | The status of the email campaign (e.g., Sent, Scheduled, Draft). | [optional] 
**date_added** | **str** | The date when the email campaign was added. | [optional] 
**custom_string** | **str** | A custom string associated with the email campaign. | [optional] 
**send_count** | **int** | The count of emails sent in the campaign. | [optional] 
**open_count** | **int** | The count of emails opened in the campaign. | [optional] 
**click_count** | **int** | The count of links clicked in the campaign. | [optional] 
**hard_bounce_count** | **int** | The count of hard bounces in the campaign. | [optional] 
**soft_bounce_count** | **int** | The count of soft bounces in the campaign. | [optional] 
**abuse_count** | **int** | The count of abuse complaints in the campaign. | [optional] 
**unsubscribe_count** | **int** | The count of unsubscribes in the campaign. | [optional] 
**body** | **str** | The body of the email campaign. | [optional] 
**body_plain_text** | **str** | The plain text body of the email campaign. | [optional] 

## Example

```python
from clicksend.models.email_campaign import EmailCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of EmailCampaign from a JSON string
email_campaign_instance = EmailCampaign.from_json(json)
# print the JSON string representation of the object
print(EmailCampaign.to_json())

# convert the object into a dict
email_campaign_dict = email_campaign_instance.to_dict()
# create an instance of EmailCampaign from a dict
email_campaign_from_dict = EmailCampaign.from_dict(email_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


