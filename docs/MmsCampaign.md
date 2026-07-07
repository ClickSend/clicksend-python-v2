# MmsCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mms_campaign_id** | **int** | The ID of the MMS campaign. | [optional] 
**name** | **str** | The name of the MMS campaign. | [optional] 
**user_id** | **int** | The ID of the user who created the campaign. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount associated with the campaign. | [optional] 
**list_id** | **int** | The ID of the list associated with the campaign. | [optional] 
**var_from** | **str** | The sender&#39;s phone number or ID. | [optional] 
**subject** | **str** | The subject of the MMS campaign. | [optional] 
**file_name** | **str** | The name of the media file attached to the MMS. | [optional] 
**body** | **str** | The body or content of the MMS. | [optional] 
**schedule** | **int** | The schedule time of the MMS campaign. | [optional] 
**status** | **str** | The status of the MMS campaign. | [optional] 
**date_added** | **int** | The date when the campaign was added. | [optional] 
**total_count** | **int** | The total count associated with the campaign. | [optional] 
**list_name** | **str** | The name of the list associated with the campaign. | [optional] 
**media_file_url** | **str** | The URL of the media file attached to the MMS. | [optional] 

## Example

```python
from clicksend.models.mms_campaign import MmsCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of MmsCampaign from a JSON string
mms_campaign_instance = MmsCampaign.from_json(json)
# print the JSON string representation of the object
print(MmsCampaign.to_json())

# convert the object into a dict
mms_campaign_dict = mms_campaign_instance.to_dict()
# create an instance of MmsCampaign from a dict
mms_campaign_from_dict = MmsCampaign.from_dict(mms_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


