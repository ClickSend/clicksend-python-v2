# SendEmailCampaignRequest


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
**custom_string** | **str** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_email_campaign_request import SendEmailCampaignRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailCampaignRequest from a JSON string
send_email_campaign_request_instance = SendEmailCampaignRequest.from_json(json)
# print the JSON string representation of the object
print(SendEmailCampaignRequest.to_json())

# convert the object into a dict
send_email_campaign_request_dict = send_email_campaign_request_instance.to_dict()
# create an instance of SendEmailCampaignRequest from a dict
send_email_campaign_request_from_dict = SendEmailCampaignRequest.from_dict(send_email_campaign_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


