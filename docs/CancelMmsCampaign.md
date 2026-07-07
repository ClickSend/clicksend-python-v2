# CancelMmsCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**MmsCampaign**](MmsCampaign.md) |  | [optional] 

## Example

```python
from clicksend.models.cancel_mms_campaign import CancelMmsCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of CancelMmsCampaign from a JSON string
cancel_mms_campaign_instance = CancelMmsCampaign.from_json(json)
# print the JSON string representation of the object
print(CancelMmsCampaign.to_json())

# convert the object into a dict
cancel_mms_campaign_dict = cancel_mms_campaign_instance.to_dict()
# create an instance of CancelMmsCampaign from a dict
cancel_mms_campaign_from_dict = CancelMmsCampaign.from_dict(cancel_mms_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


