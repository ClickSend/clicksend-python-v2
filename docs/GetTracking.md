# GetTracking


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **float** | Total number of short URLs associated with the long URL ID | [optional] 
**per_page** | **float** | The limit of tracking data per page | [optional] 
**current_page_size** | **float** | The number of data in the current page | [optional] 
**prev_page_url** | **str** | Link to the previous page. This attribute will not be present if there is no previous page. | [optional] 
**next_page_url** | **str** | Link to the next page. This attribute will not be present if there is no next page. | [optional] 
**data** | [**List[GetTrackingDataInner]**](GetTrackingDataInner.md) | Tracking data of the short URLs associated with the specified long URL ID. Note that only the data from the most recent click of the recipient (country, region, device, browser, and os) is recorded. | [optional] 

## Example

```python
from clicksend.models.get_tracking import GetTracking

# TODO update the JSON string below
json = "{}"
# create an instance of GetTracking from a JSON string
get_tracking_instance = GetTracking.from_json(json)
# print the JSON string representation of the object
print(GetTracking.to_json())

# convert the object into a dict
get_tracking_dict = get_tracking_instance.to_dict()
# create an instance of GetTracking from a dict
get_tracking_from_dict = GetTracking.from_dict(get_tracking_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


