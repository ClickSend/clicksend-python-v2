# Account


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | The unique identifier for the user. | [optional] 
**username** | **str** | The username of the user. | [optional] 
**user_email** | **str** | The email address of the user. | [optional] 
**active** | **int** | Flag indicating if the user account is active. | [optional] 
**banned** | **int** | Flag indicating if the user account is banned. | [optional] 
**balance** | **str** | The balance of the user&#39;s account. | [optional] 
**user_phone** | **str** | The phone number of the user. | [optional] 
**reply_to** | **str** | The email address to reply to. | [optional] 
**delivery_to** | **str** | The delivery email address. | [optional] 
**user_first_name** | **str** | The first name of the user. | [optional] 
**user_last_name** | **str** | The last name of the user. | [optional] 
**account** | **int** | The account number. | [optional] 
**account_name** | **str** | The name of the account. | [optional] 
**account_billing_email** | **str** | The billing email address of the account. | [optional] 
**account_billing_mobile** | **str** | The billing mobile number of the account. | [optional] 
**country** | **str** | The country of the user. | [optional] 
**default_country_sms** | **str** | The default country for SMS. | [optional] 
**auto_recharge** | **int** | Flag indicating if auto-recharge is enabled. | [optional] 
**auto_recharge_amount** | **str** | The auto-recharge amount. | [optional] 
**low_credit_amount** | **str** | The low credit amount. | [optional] 
**setting_unicode_sms** | **int** | Flag indicating if unicode SMS is enabled. | [optional] 
**setting_email_sms_subject** | **int** | Flag indicating if email SMS subject is enabled. | [optional] 
**setting_fix_sender_id** | **int** | Flag indicating if fixing sender ID is enabled. | [optional] 
**setting_sms_message_char_limit** | **int** | The SMS message character limit. | [optional] 
**old_dashboard** | **int** | Flag indicating if old dashboard is enabled. | [optional] 
**balance_commission** | **str** | The balance commission. | [optional] 
**timezone** | **str** | The timezone of the user. | [optional] 
**price_rate** | **int** | The pricing tier used to determine the cost per message. | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 
**subaccount** | [**Subaccount**](Subaccount.md) |  | [optional] 

## Example

```python
from clicksend.models.account import Account

# TODO update the JSON string below
json = "{}"
# create an instance of Account from a JSON string
account_instance = Account.from_json(json)
# print the JSON string representation of the object
print(Account.to_json())

# convert the object into a dict
account_dict = account_instance.to_dict()
# create an instance of Account from a dict
account_from_dict = Account.from_dict(account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


