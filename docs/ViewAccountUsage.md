# ViewAccountUsage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewAccountUsageData**](ViewAccountUsageData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_account_usage import ViewAccountUsage

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsage from a JSON string
view_account_usage_instance = ViewAccountUsage.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsage.to_json())

# convert the object into a dict
view_account_usage_dict = view_account_usage_instance.to_dict()
# create an instance of ViewAccountUsage from a dict
view_account_usage_from_dict = ViewAccountUsage.from_dict(view_account_usage_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


