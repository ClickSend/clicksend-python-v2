# ViewSubaccounts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewSubaccountsData**](ViewSubaccountsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_subaccounts import ViewSubaccounts

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSubaccounts from a JSON string
view_subaccounts_instance = ViewSubaccounts.from_json(json)
# print the JSON string representation of the object
print(ViewSubaccounts.to_json())

# convert the object into a dict
view_subaccounts_dict = view_subaccounts_instance.to_dict()
# create an instance of ViewSubaccounts from a dict
view_subaccounts_from_dict = ViewSubaccounts.from_dict(view_subaccounts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


