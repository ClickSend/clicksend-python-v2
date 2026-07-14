# ViewAccountUsageDataEmailInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subaccount_id** | **int** | The subaccount identifier. | [optional] 
**username** | **str** | The username associated with the subaccount. | [optional] 
**total_count** | **int** | The total count of emails. | [optional] 
**total_price** | **str** |  | [optional] 
**notes** | **str** | Optional notes. | [optional] 

## Example

```python
from clicksend.models.view_account_usage_data_email_inner import ViewAccountUsageDataEmailInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsageDataEmailInner from a JSON string
view_account_usage_data_email_inner_instance = ViewAccountUsageDataEmailInner.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsageDataEmailInner.to_json())

# convert the object into a dict
view_account_usage_data_email_inner_dict = view_account_usage_data_email_inner_instance.to_dict()
# create an instance of ViewAccountUsageDataEmailInner from a dict
view_account_usage_data_email_inner_from_dict = ViewAccountUsageDataEmailInner.from_dict(view_account_usage_data_email_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


