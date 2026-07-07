# ViewReferralAccounts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewReferralAccountsData**](ViewReferralAccountsData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_referral_accounts import ViewReferralAccounts

# TODO update the JSON string below
json = "{}"
# create an instance of ViewReferralAccounts from a JSON string
view_referral_accounts_instance = ViewReferralAccounts.from_json(json)
# print the JSON string representation of the object
print(ViewReferralAccounts.to_json())

# convert the object into a dict
view_referral_accounts_dict = view_referral_accounts_instance.to_dict()
# create an instance of ViewReferralAccounts from a dict
view_referral_accounts_from_dict = ViewReferralAccounts.from_dict(view_referral_accounts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


