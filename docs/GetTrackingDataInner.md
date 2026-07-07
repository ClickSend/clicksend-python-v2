# GetTrackingDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**open_count** | **float** | Number of times the short URL was opened | [optional] 
**date_opened** | **float** | Date in unix seconds when the short URL was first opened. Null if the short URL was never opened. | [optional] 
**user_geo_country** | **str** | Country where the recipient is located when the short URL was opened. Null if the short URL was never opened. | [optional] 
**user_geo_region** | **str** | Geographical region where the recipient is located when the short URL was opened. Null if the short URL was never opened. | [optional] 
**user_device** | **str** | Deviced used by the recipient to open the short URL. Null if the short URL was never opened. | [optional] 
**user_browser** | **str** | Browser used by the recipient to open the short URL. Null if the short URL was never opened. | [optional] 
**user_os** | **str** | Opearating system used by the recipient to open the short URL. Null if the short URL was never opened. | [optional] 
**contact** | [**GetTrackingDataInnerContact**](GetTrackingDataInnerContact.md) |  | [optional] 

## Example

```python
from clicksend.models.get_tracking_data_inner import GetTrackingDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetTrackingDataInner from a JSON string
get_tracking_data_inner_instance = GetTrackingDataInner.from_json(json)
# print the JSON string representation of the object
print(GetTrackingDataInner.to_json())

# convert the object into a dict
get_tracking_data_inner_dict = get_tracking_data_inner_instance.to_dict()
# create an instance of GetTrackingDataInner from a dict
get_tracking_data_inner_from_dict = GetTrackingDataInner.from_dict(get_tracking_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


