# GetStatisticsDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**long_url_id** | **str** | ID of a URL under the specified source and source_id | [optional] 
**links** | [**GetStatisticsDataInnerLinks**](GetStatisticsDataInnerLinks.md) |  | [optional] 
**device** | [**List[GetStatisticsDataInnerDeviceInner]**](GetStatisticsDataInnerDeviceInner.md) | Device statistics of the recipients that clicked the short URL | [optional] 
**os** | [**List[GetStatisticsDataInnerDeviceInner]**](GetStatisticsDataInnerDeviceInner.md) | OS statistics of the recipients that clicked the short URL | [optional] 
**browser** | [**List[GetStatisticsDataInnerDeviceInner]**](GetStatisticsDataInnerDeviceInner.md) | Browser statistics of the recipients that clicked the short URL | [optional] 
**country** | [**List[GetStatisticsDataInnerDeviceInner]**](GetStatisticsDataInnerDeviceInner.md) | Country statistics of the recipients that clicked the short URL | [optional] 
**region** | [**List[GetStatisticsDataInnerDeviceInner]**](GetStatisticsDataInnerDeviceInner.md) | Region statistics of the recipients that clicked the short URL | [optional] 

## Example

```python
from clicksend.models.get_statistics_data_inner import GetStatisticsDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetStatisticsDataInner from a JSON string
get_statistics_data_inner_instance = GetStatisticsDataInner.from_json(json)
# print the JSON string representation of the object
print(GetStatisticsDataInner.to_json())

# convert the object into a dict
get_statistics_data_inner_dict = get_statistics_data_inner_instance.to_dict()
# create an instance of GetStatisticsDataInner from a dict
get_statistics_data_inner_from_dict = GetStatisticsDataInner.from_dict(get_statistics_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


