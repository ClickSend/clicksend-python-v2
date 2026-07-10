# ViewVoiceStatisticsDataStatsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **float** | The date. | [optional] 
**outbound** | [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**bounced** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_voice_statistics_data_stats_inner import ViewVoiceStatisticsDataStatsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewVoiceStatisticsDataStatsInner from a JSON string
view_voice_statistics_data_stats_inner_instance = ViewVoiceStatisticsDataStatsInner.from_json(json)
# print the JSON string representation of the object
print(ViewVoiceStatisticsDataStatsInner.to_json())

# convert the object into a dict
view_voice_statistics_data_stats_inner_dict = view_voice_statistics_data_stats_inner_instance.to_dict()
# create an instance of ViewVoiceStatisticsDataStatsInner from a dict
view_voice_statistics_data_stats_inner_from_dict = ViewVoiceStatisticsDataStatsInner.from_dict(view_voice_statistics_data_stats_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


