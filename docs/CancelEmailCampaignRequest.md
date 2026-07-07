# CancelEmailCampaignRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**from_email_address_id** | **int** |  | [optional] 
**template_id** | **int** |  | [optional] 
**list_id** | **int** |  | [optional] 
**from_name** | **str** |  | [optional] 
**draft** | **int** |  | [optional] 
**schedule** | **str** |  | [optional] 
**custom_string** | **str** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from clicksend.models.cancel_email_campaign_request import CancelEmailCampaignRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CancelEmailCampaignRequest from a JSON string
cancel_email_campaign_request_instance = CancelEmailCampaignRequest.from_json(json)
# print the JSON string representation of the object
print(CancelEmailCampaignRequest.to_json())

# convert the object into a dict
cancel_email_campaign_request_dict = cancel_email_campaign_request_instance.to_dict()
# create an instance of CancelEmailCampaignRequest from a dict
cancel_email_campaign_request_from_dict = CancelEmailCampaignRequest.from_dict(cancel_email_campaign_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


