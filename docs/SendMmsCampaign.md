# SendMmsCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**MmsCampaign**](MmsCampaign.md) |  | [optional] 

## Example

```python
from clicksend.models.send_mms_campaign import SendMmsCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of SendMmsCampaign from a JSON string
send_mms_campaign_instance = SendMmsCampaign.from_json(json)
# print the JSON string representation of the object
print(SendMmsCampaign.to_json())

# convert the object into a dict
send_mms_campaign_dict = send_mms_campaign_instance.to_dict()
# create an instance of SendMmsCampaign from a dict
send_mms_campaign_from_dict = SendMmsCampaign.from_dict(send_mms_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


