# GetAllDeliveryIssuesData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** | The total number of items available for viewing. | [optional] 
**per_page** | **int** | The number of items returned per page. This is specified in the limit parameter. You can have 100 items at maximum, and 15 at minimum. | [optional] 
**current_page** | **int** | The current page number. | [optional] 
**last_page** | **int** | The last page number. | [optional] 
**next_page_url** | **str** | A URL of the next page. It will return **null** if there’s no next page. | [optional] 
**prev_page_url** | **str** | A URL of the previous page. It will return **null** if there’s no previous page. | [optional] 
**var_from** | **int** | The number of the first result in the current page. | [optional] 
**to** | **int** | The number of the last result in the current page. | [optional] 
**data** | [**List[DeliveryIssue]**](DeliveryIssue.md) |  | [optional] 

## Example

```python
from clicksend.models.get_all_delivery_issues_data import GetAllDeliveryIssuesData

# TODO update the JSON string below
json = "{}"
# create an instance of GetAllDeliveryIssuesData from a JSON string
get_all_delivery_issues_data_instance = GetAllDeliveryIssuesData.from_json(json)
# print the JSON string representation of the object
print(GetAllDeliveryIssuesData.to_json())

# convert the object into a dict
get_all_delivery_issues_data_dict = get_all_delivery_issues_data_instance.to_dict()
# create an instance of GetAllDeliveryIssuesData from a dict
get_all_delivery_issues_data_from_dict = GetAllDeliveryIssuesData.from_dict(get_all_delivery_issues_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


