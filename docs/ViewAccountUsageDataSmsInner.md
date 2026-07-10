# ViewAccountUsageDataSmsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subaccount_id** | **int** | The subaccount identifier. | [optional] 
**username** | **str** | The username associated with the subaccount. | [optional] 
**total_count** | **str** | The total count of SMS. | [optional] 
**total_price** | **float** | The total price of SMS. | [optional] 

## Example

```python
from clicksend.models.view_account_usage_data_sms_inner import ViewAccountUsageDataSmsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsageDataSmsInner from a JSON string
view_account_usage_data_sms_inner_instance = ViewAccountUsageDataSmsInner.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsageDataSmsInner.to_json())

# convert the object into a dict
view_account_usage_data_sms_inner_dict = view_account_usage_data_sms_inner_instance.to_dict()
# create an instance of ViewAccountUsageDataSmsInner from a dict
view_account_usage_data_sms_inner_from_dict = ViewAccountUsageDataSmsInner.from_dict(view_account_usage_data_sms_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


