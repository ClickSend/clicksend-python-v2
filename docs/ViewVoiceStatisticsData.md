# ViewVoiceStatisticsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | [**ViewVoiceStatisticsDataTotal**](ViewVoiceStatisticsDataTotal.md) |  | [optional] 
**stats** | [**List[ViewVoiceStatisticsDataStatsInner]**](ViewVoiceStatisticsDataStatsInner.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.view_voice_statistics_data import ViewVoiceStatisticsData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewVoiceStatisticsData from a JSON string
view_voice_statistics_data_instance = ViewVoiceStatisticsData.from_json(json)
# print the JSON string representation of the object
print(ViewVoiceStatisticsData.to_json())

# convert the object into a dict
view_voice_statistics_data_dict = view_voice_statistics_data_instance.to_dict()
# create an instance of ViewVoiceStatisticsData from a dict
view_voice_statistics_data_from_dict = ViewVoiceStatisticsData.from_dict(view_voice_statistics_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


