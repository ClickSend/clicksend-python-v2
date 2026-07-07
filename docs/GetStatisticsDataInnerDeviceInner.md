# GetStatisticsDataInnerDeviceInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **str** | Device name | [optional] 
**count** | **float** | Total number of clicks on the short URL where the recipient has the specified device name | [optional] 

## Example

```python
from clicksend.models.get_statistics_data_inner_device_inner import GetStatisticsDataInnerDeviceInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetStatisticsDataInnerDeviceInner from a JSON string
get_statistics_data_inner_device_inner_instance = GetStatisticsDataInnerDeviceInner.from_json(json)
# print the JSON string representation of the object
print(GetStatisticsDataInnerDeviceInner.to_json())

# convert the object into a dict
get_statistics_data_inner_device_inner_dict = get_statistics_data_inner_device_inner_instance.to_dict()
# create an instance of GetStatisticsDataInnerDeviceInner from a dict
get_statistics_data_inner_device_inner_from_dict = GetStatisticsDataInnerDeviceInner.from_dict(get_statistics_data_inner_device_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


