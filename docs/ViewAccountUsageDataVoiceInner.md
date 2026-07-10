# ViewAccountUsageDataVoiceInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subaccount_id** | **int** | The subaccount identifier. | [optional] 
**username** | **str** | The username associated with the subaccount. | [optional] 
**total_count** | **str** | The total count of voice calls. | [optional] 
**total_price** | **str** | The total price of voice calls. | [optional] 

## Example

```python
from clicksend.models.view_account_usage_data_voice_inner import ViewAccountUsageDataVoiceInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsageDataVoiceInner from a JSON string
view_account_usage_data_voice_inner_instance = ViewAccountUsageDataVoiceInner.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsageDataVoiceInner.to_json())

# convert the object into a dict
view_account_usage_data_voice_inner_dict = view_account_usage_data_voice_inner_instance.to_dict()
# create an instance of ViewAccountUsageDataVoiceInner from a dict
view_account_usage_data_voice_inner_from_dict = ViewAccountUsageDataVoiceInner.from_dict(view_account_usage_data_voice_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


