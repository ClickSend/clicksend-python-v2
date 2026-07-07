# CancelEmailCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**EmailCampaign**](EmailCampaign.md) |  | [optional] 

## Example

```python
from clicksend.models.cancel_email_campaign import CancelEmailCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of CancelEmailCampaign from a JSON string
cancel_email_campaign_instance = CancelEmailCampaign.from_json(json)
# print the JSON string representation of the object
print(CancelEmailCampaign.to_json())

# convert the object into a dict
cancel_email_campaign_dict = cancel_email_campaign_instance.to_dict()
# create an instance of CancelEmailCampaign from a dict
cancel_email_campaign_from_dict = CancelEmailCampaign.from_dict(cancel_email_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


