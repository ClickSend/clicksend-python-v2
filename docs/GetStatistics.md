# GetStatistics


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GetStatisticsDataInner]**](GetStatisticsDataInner.md) |  | [optional] 

## Example

```python
from clicksend.models.get_statistics import GetStatistics

# TODO update the JSON string below
json = "{}"
# create an instance of GetStatistics from a JSON string
get_statistics_instance = GetStatistics.from_json(json)
# print the JSON string representation of the object
print(GetStatistics.to_json())

# convert the object into a dict
get_statistics_dict = get_statistics_instance.to_dict()
# create an instance of GetStatistics from a dict
get_statistics_from_dict = GetStatistics.from_dict(get_statistics_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


