# SendMmsCampaignRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**list_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**url_to_shorten** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**media_file** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_mms_campaign_request import SendMmsCampaignRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendMmsCampaignRequest from a JSON string
send_mms_campaign_request_instance = SendMmsCampaignRequest.from_json(json)
# print the JSON string representation of the object
print(SendMmsCampaignRequest.to_json())

# convert the object into a dict
send_mms_campaign_request_dict = send_mms_campaign_request_instance.to_dict()
# create an instance of SendMmsCampaignRequest from a dict
send_mms_campaign_request_from_dict = SendMmsCampaignRequest.from_dict(send_mms_campaign_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


