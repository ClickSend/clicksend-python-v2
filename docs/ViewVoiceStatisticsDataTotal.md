# ViewVoiceStatisticsDataTotal


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**outbound** | [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**bounced** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_voice_statistics_data_total import ViewVoiceStatisticsDataTotal

# TODO update the JSON string below
json = "{}"
# create an instance of ViewVoiceStatisticsDataTotal from a JSON string
view_voice_statistics_data_total_instance = ViewVoiceStatisticsDataTotal.from_json(json)
# print the JSON string representation of the object
print(ViewVoiceStatisticsDataTotal.to_json())

# convert the object into a dict
view_voice_statistics_data_total_dict = view_voice_statistics_data_total_instance.to_dict()
# create an instance of ViewVoiceStatisticsDataTotal from a dict
view_voice_statistics_data_total_from_dict = ViewVoiceStatisticsDataTotal.from_dict(view_voice_statistics_data_total_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


