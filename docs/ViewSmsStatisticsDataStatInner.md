# ViewSmsStatisticsDataStatInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **float** | The date. | [optional] 
**outbound** | [**ViewVoiceStatisticsDataStatsInnerOutbound**](ViewVoiceStatisticsDataStatsInnerOutbound.md) |  | [optional] 
**inbound** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 
**bounced** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_statistics_data_stat_inner import ViewSmsStatisticsDataStatInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsStatisticsDataStatInner from a JSON string
view_sms_statistics_data_stat_inner_instance = ViewSmsStatisticsDataStatInner.from_json(json)
# print the JSON string representation of the object
print(ViewSmsStatisticsDataStatInner.to_json())

# convert the object into a dict
view_sms_statistics_data_stat_inner_dict = view_sms_statistics_data_stat_inner_instance.to_dict()
# create an instance of ViewSmsStatisticsDataStatInner from a dict
view_sms_statistics_data_stat_inner_from_dict = ViewSmsStatisticsDataStatInner.from_dict(view_sms_statistics_data_stat_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


