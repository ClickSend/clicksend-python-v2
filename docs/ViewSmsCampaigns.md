# ViewSmsCampaigns


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewSmsCampaignsData**](ViewSmsCampaignsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_campaigns import ViewSmsCampaigns

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsCampaigns from a JSON string
view_sms_campaigns_instance = ViewSmsCampaigns.from_json(json)
# print the JSON string representation of the object
print(ViewSmsCampaigns.to_json())

# convert the object into a dict
view_sms_campaigns_dict = view_sms_campaigns_instance.to_dict()
# create an instance of ViewSmsCampaigns from a dict
view_sms_campaigns_from_dict = ViewSmsCampaigns.from_dict(view_sms_campaigns_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


