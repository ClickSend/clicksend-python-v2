# Account


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | The unique identifier for the user. | [optional] 
**username** | **str** | The username of the user. | [optional] 
**user_email** | **str** | The email address of the user. | [optional] 
**active** | **int** | Flag indicating if the user account is active. | [optional] 
**banned** | **int** | Flag indicating if the user account is banned. | [optional] 
**date_sign_up** | **int** | The Unix timestamp of when the account was created. | [optional] 
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
**priority** | **int** | The account&#39;s priority tier. | [optional] 
**country** | **str** | The country of the user. | [optional] 
**country_ip** | **str** | The country the user is currently connecting from, based on IP address. | [optional] 
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
**private_uploads** | **int** | Flag indicating if uploaded media is kept private. | [optional] 
**fax_quality** | **int** | The quality setting used for outgoing faxes. | [optional] 
**setting_sms_hide_your_number** | **int** | Flag indicating if your number is hidden on outgoing SMS. | [optional] 
**setting_sms_hide_business_name** | **int** | Flag indicating if the business name is hidden on outgoing SMS. | [optional] 
**pricing_variant** | **int** | The pricing variant applied to the account. | [optional] 
**on_trial** | **int** | Flag indicating if the account is currently on a trial. | [optional] 
**trial_expiry** | **str** | The date the trial expires, if the account is on a trial. | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 
**subaccount** | [**Subaccount**](Subaccount.md) |  | [optional] 
**referrer_chosen** | [**AccountReferrerChosen**](AccountReferrerChosen.md) |  | [optional] 

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


