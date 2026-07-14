# ViewSmsStatisticsDataStatsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **float** | The date. | [optional] 
**outbound** | [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**inbound** | [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**bounced** | [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_statistics_data_stats_inner import ViewSmsStatisticsDataStatsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsStatisticsDataStatsInner from a JSON string
view_sms_statistics_data_stats_inner_instance = ViewSmsStatisticsDataStatsInner.from_json(json)
# print the JSON string representation of the object
print(ViewSmsStatisticsDataStatsInner.to_json())

# convert the object into a dict
view_sms_statistics_data_stats_inner_dict = view_sms_statistics_data_stats_inner_instance.to_dict()
# create an instance of ViewSmsStatisticsDataStatsInner from a dict
view_sms_statistics_data_stats_inner_from_dict = ViewSmsStatisticsDataStatsInner.from_dict(view_sms_statistics_data_stats_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


