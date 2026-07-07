# ViewAccountUsageData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sms** | [**List[ViewAccountUsageDataSmsInner]**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**voice** | [**List[ViewAccountUsageDataSmsInner]**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**fax** | [**List[ViewAccountUsageDataSmsInner]**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**post** | [**List[ViewAccountUsageDataSmsInner]**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**email** | [**List[ViewAccountUsageDataEmailInner]**](ViewAccountUsageDataEmailInner.md) |  | [optional] 
**sms_total** | [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**voice_total** | [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**fax_total** | [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**post_total** | [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**email_total** | [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 

## Example

```python
from clicksend.models.view_account_usage_data import ViewAccountUsageData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsageData from a JSON string
view_account_usage_data_instance = ViewAccountUsageData.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsageData.to_json())

# convert the object into a dict
view_account_usage_data_dict = view_account_usage_data_instance.to_dict()
# create an instance of ViewAccountUsageData from a dict
view_account_usage_data_from_dict = ViewAccountUsageData.from_dict(view_account_usage_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


