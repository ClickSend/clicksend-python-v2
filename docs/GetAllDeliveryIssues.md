# GetAllDeliveryIssues


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**GetAllDeliveryIssuesData**](GetAllDeliveryIssuesData.md) |  | [optional] 

## Example

```python
from clicksend.models.get_all_delivery_issues import GetAllDeliveryIssues

# TODO update the JSON string below
json = "{}"
# create an instance of GetAllDeliveryIssues from a JSON string
get_all_delivery_issues_instance = GetAllDeliveryIssues.from_json(json)
# print the JSON string representation of the object
print(GetAllDeliveryIssues.to_json())

# convert the object into a dict
get_all_delivery_issues_dict = get_all_delivery_issues_instance.to_dict()
# create an instance of GetAllDeliveryIssues from a dict
get_all_delivery_issues_from_dict = GetAllDeliveryIssues.from_dict(get_all_delivery_issues_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


