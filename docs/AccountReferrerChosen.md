# AccountReferrerChosen

The referral source chosen at sign-up, if any.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the referral source. | [optional] 
**name** | **str** | The name of the referral source. | [optional] 

## Example

```python
from clicksend.models.account_referrer_chosen import AccountReferrerChosen

# TODO update the JSON string below
json = "{}"
# create an instance of AccountReferrerChosen from a JSON string
account_referrer_chosen_instance = AccountReferrerChosen.from_json(json)
# print the JSON string representation of the object
print(AccountReferrerChosen.to_json())

# convert the object into a dict
account_referrer_chosen_dict = account_referrer_chosen_instance.to_dict()
# create an instance of AccountReferrerChosen from a dict
account_referrer_chosen_from_dict = AccountReferrerChosen.from_dict(account_referrer_chosen_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


