# ViewAccountUsageDataSmsTotal


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **str** | The total count of SMS. | [optional] 
**price** | **str** | The total price of SMS. | [optional] 

## Example

```python
from clicksend.models.view_account_usage_data_sms_total import ViewAccountUsageDataSmsTotal

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsageDataSmsTotal from a JSON string
view_account_usage_data_sms_total_instance = ViewAccountUsageDataSmsTotal.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsageDataSmsTotal.to_json())

# convert the object into a dict
view_account_usage_data_sms_total_dict = view_account_usage_data_sms_total_instance.to_dict()
# create an instance of ViewAccountUsageDataSmsTotal from a dict
view_account_usage_data_sms_total_from_dict = ViewAccountUsageDataSmsTotal.from_dict(view_account_usage_data_sms_total_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


