# ViewSmsStatisticsDataTotal


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**outbound** | [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**inbound** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 
**bounced** | [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_statistics_data_total import ViewSmsStatisticsDataTotal

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsStatisticsDataTotal from a JSON string
view_sms_statistics_data_total_instance = ViewSmsStatisticsDataTotal.from_json(json)
# print the JSON string representation of the object
print(ViewSmsStatisticsDataTotal.to_json())

# convert the object into a dict
view_sms_statistics_data_total_dict = view_sms_statistics_data_total_instance.to_dict()
# create an instance of ViewSmsStatisticsDataTotal from a dict
view_sms_statistics_data_total_from_dict = ViewSmsStatisticsDataTotal.from_dict(view_sms_statistics_data_total_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


