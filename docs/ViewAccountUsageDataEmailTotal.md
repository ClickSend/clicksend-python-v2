# ViewAccountUsageDataEmailTotal


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **int** | The total count of emails. | [optional] 
**price** | **str** | The total price of emails. | [optional] 

## Example

```python
from clicksend.models.view_account_usage_data_email_total import ViewAccountUsageDataEmailTotal

# TODO update the JSON string below
json = "{}"
# create an instance of ViewAccountUsageDataEmailTotal from a JSON string
view_account_usage_data_email_total_instance = ViewAccountUsageDataEmailTotal.from_json(json)
# print the JSON string representation of the object
print(ViewAccountUsageDataEmailTotal.to_json())

# convert the object into a dict
view_account_usage_data_email_total_dict = view_account_usage_data_email_total_instance.to_dict()
# create an instance of ViewAccountUsageDataEmailTotal from a dict
view_account_usage_data_email_total_from_dict = ViewAccountUsageDataEmailTotal.from_dict(view_account_usage_data_email_total_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


