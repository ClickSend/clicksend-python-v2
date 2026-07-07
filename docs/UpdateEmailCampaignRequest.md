# UpdateEmailCampaignRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**schedule** | **int** |  | [optional] 
**list_id** | **int** |  | [optional] 
**subject** | **str** |  | [optional] 
**from_email_address_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**template_id** | **int** |  | [optional] 
**body** | **str** |  | [optional] 
**from_name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.update_email_campaign_request import UpdateEmailCampaignRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateEmailCampaignRequest from a JSON string
update_email_campaign_request_instance = UpdateEmailCampaignRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateEmailCampaignRequest.to_json())

# convert the object into a dict
update_email_campaign_request_dict = update_email_campaign_request_instance.to_dict()
# create an instance of UpdateEmailCampaignRequest from a dict
update_email_campaign_request_from_dict = UpdateEmailCampaignRequest.from_dict(update_email_campaign_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


