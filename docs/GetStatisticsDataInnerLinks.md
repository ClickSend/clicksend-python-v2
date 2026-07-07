# GetStatisticsDataInnerLinks

Link statistics

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **float** | Total number of recipients | [optional] 
**opened_unique** | **float** | Total number of recipients that clicked the short URL | [optional] 
**opened_total** | **float** | Total number of clicks on the short URL (e.g. when a recipient clicked the short URL twice, then it will add 2 here) | [optional] 
**unopened** | **float** | Total number of recipients that did not click the short URL (i.e. &#x60;total&#x60; - &#x60;opened_unique&#x60;) | [optional] 

## Example

```python
from clicksend.models.get_statistics_data_inner_links import GetStatisticsDataInnerLinks

# TODO update the JSON string below
json = "{}"
# create an instance of GetStatisticsDataInnerLinks from a JSON string
get_statistics_data_inner_links_instance = GetStatisticsDataInnerLinks.from_json(json)
# print the JSON string representation of the object
print(GetStatisticsDataInnerLinks.to_json())

# convert the object into a dict
get_statistics_data_inner_links_dict = get_statistics_data_inner_links_instance.to_dict()
# create an instance of GetStatisticsDataInnerLinks from a dict
get_statistics_data_inner_links_from_dict = GetStatisticsDataInnerLinks.from_dict(get_statistics_data_inner_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


