# ViewSmsStatisticsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | [**ViewSmsStatisticsDataTotal**](ViewSmsStatisticsDataTotal.md) |  | [optional] 
**stats** | [**List[ViewSmsStatisticsDataStatsInner]**](ViewSmsStatisticsDataStatsInner.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_statistics_data import ViewSmsStatisticsData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsStatisticsData from a JSON string
view_sms_statistics_data_instance = ViewSmsStatisticsData.from_json(json)
# print the JSON string representation of the object
print(ViewSmsStatisticsData.to_json())

# convert the object into a dict
view_sms_statistics_data_dict = view_sms_statistics_data_instance.to_dict()
# create an instance of ViewSmsStatisticsData from a dict
view_sms_statistics_data_from_dict = ViewSmsStatisticsData.from_dict(view_sms_statistics_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


