# ViewAllEmailCampaigns


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewAllEmailCampaignsData**](ViewAllEmailCampaignsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_all_email_campaigns import ViewAllEmailCampaigns

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAllEmailCampaigns from a JSON string
view_all_email_campaigns_instance = ViewAllEmailCampaigns.from_json(json)
# print the JSON string representation of the object
print(ViewAllEmailCampaigns.to_json())

# convert the object into a dict
view_all_email_campaigns_dict = view_all_email_campaigns_instance.to_dict()
# create an instance of ViewAllEmailCampaigns from a dict
view_all_email_campaigns_from_dict = ViewAllEmailCampaigns.from_dict(view_all_email_campaigns_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


