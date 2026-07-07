# ViewReferralAccountsDataAllOfDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**referral_rule_id** | **int** | The ID of the Referral Account. | [optional] 
**refered_user_id** | **int** | The ID of the Referral Account. | [optional] 
**date_referred** | **float** | The ID of the Referral Account. | [optional] 
**percentage_referral** | **float** | The Percentage of the Referral. | [optional] 

## Example

```python
from clicksend.models.view_referral_accounts_data_all_of_data_inner import ViewReferralAccountsDataAllOfDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewReferralAccountsDataAllOfDataInner from a JSON string
view_referral_accounts_data_all_of_data_inner_instance = ViewReferralAccountsDataAllOfDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewReferralAccountsDataAllOfDataInner.to_json())

# convert the object into a dict
view_referral_accounts_data_all_of_data_inner_dict = view_referral_accounts_data_all_of_data_inner_instance.to_dict()
# create an instance of ViewReferralAccountsDataAllOfDataInner from a dict
view_referral_accounts_data_all_of_data_inner_from_dict = ViewReferralAccountsDataAllOfDataInner.from_dict(view_referral_accounts_data_all_of_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


