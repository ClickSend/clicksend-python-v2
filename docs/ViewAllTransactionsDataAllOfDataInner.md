# ViewAllTransactionsDataAllOfDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_number** | **str** | The invoice number. | [optional] 
**amount** | **float** | The amount of the transaction. | [optional] 
**currency** | **str** | The currency of the transaction. | [optional] 
**var_date** | **float** | The date of the transaction. | [optional] 

## Example

```python
from clicksend.models.view_all_transactions_data_all_of_data_inner import ViewAllTransactionsDataAllOfDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAllTransactionsDataAllOfDataInner from a JSON string
view_all_transactions_data_all_of_data_inner_instance = ViewAllTransactionsDataAllOfDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewAllTransactionsDataAllOfDataInner.to_json())

# convert the object into a dict
view_all_transactions_data_all_of_data_inner_dict = view_all_transactions_data_all_of_data_inner_instance.to_dict()
# create an instance of ViewAllTransactionsDataAllOfDataInner from a dict
view_all_transactions_data_all_of_data_inner_from_dict = ViewAllTransactionsDataAllOfDataInner.from_dict(view_all_transactions_data_all_of_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


