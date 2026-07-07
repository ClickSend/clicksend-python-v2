# ViewAllTransactions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewAllTransactionsData**](ViewAllTransactionsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_all_transactions import ViewAllTransactions

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAllTransactions from a JSON string
view_all_transactions_instance = ViewAllTransactions.from_json(json)
# print the JSON string representation of the object
print(ViewAllTransactions.to_json())

# convert the object into a dict
view_all_transactions_dict = view_all_transactions_instance.to_dict()
# create an instance of ViewAllTransactions from a dict
view_all_transactions_from_dict = ViewAllTransactions.from_dict(view_all_transactions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


