# CancelSmsCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SmsCampaign**](SmsCampaign.md) |  | [optional] 

## Example

```python
from clicksend.models.cancel_sms_campaign import CancelSmsCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of CancelSmsCampaign from a JSON string
cancel_sms_campaign_instance = CancelSmsCampaign.from_json(json)
# print the JSON string representation of the object
print(CancelSmsCampaign.to_json())

# convert the object into a dict
cancel_sms_campaign_dict = cancel_sms_campaign_instance.to_dict()
# create an instance of CancelSmsCampaign from a dict
cancel_sms_campaign_from_dict = CancelSmsCampaign.from_dict(cancel_sms_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


