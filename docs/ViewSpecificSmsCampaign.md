# ViewSpecificSmsCampaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SmsCampaign**](SmsCampaign.md) |  | [optional] 

## Example

```python
from clicksend.models.view_specific_sms_campaign import ViewSpecificSmsCampaign

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSpecificSmsCampaign from a JSON string
view_specific_sms_campaign_instance = ViewSpecificSmsCampaign.from_json(json)
# print the JSON string representation of the object
print(ViewSpecificSmsCampaign.to_json())

# convert the object into a dict
view_specific_sms_campaign_dict = view_specific_sms_campaign_instance.to_dict()
# create an instance of ViewSpecificSmsCampaign from a dict
view_specific_sms_campaign_from_dict = ViewSpecificSmsCampaign.from_dict(view_specific_sms_campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


