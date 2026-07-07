# ViewMmsCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**MmsCampaign**](MmsCampaign.md) |  | [optional] 

## Example

```python
from clicksend.models.view_mms_campaign import ViewMmsCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of ViewMmsCampaign from a JSON string
view_mms_campaign_instance = ViewMmsCampaign.from_json(json)
# print the JSON string representation of the object
print(ViewMmsCampaign.to_json())

# convert the object into a dict
view_mms_campaign_dict = view_mms_campaign_instance.to_dict()
# create an instance of ViewMmsCampaign from a dict
view_mms_campaign_from_dict = ViewMmsCampaign.from_dict(view_mms_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


