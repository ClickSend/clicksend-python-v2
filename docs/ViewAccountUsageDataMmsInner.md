# ViewAccountUsageDataMmsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subaccount_id** | **int** | The subaccount identifier. | [optional] 
**username** | **str** | The username associated with the subaccount. | [optional] 
**total_count** | **str** | The total count of MMS. | [optional] 
**total_price** | **str** | The total price of MMS. | [optional] 
**notes** | **str** | Optional notes. | [optional] 

## Example

```python
from clicksend.models.view_account_usage_data_mms_inner import ViewAccountUsageDataMmsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsageDataMmsInner from a JSON string
view_account_usage_data_mms_inner_instance = ViewAccountUsageDataMmsInner.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsageDataMmsInner.to_json())

# convert the object into a dict
view_account_usage_data_mms_inner_dict = view_account_usage_data_mms_inner_instance.to_dict()
# create an instance of ViewAccountUsageDataMmsInner from a dict
view_account_usage_data_mms_inner_from_dict = ViewAccountUsageDataMmsInner.from_dict(view_account_usage_data_mms_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


