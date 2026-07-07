# CreateResellerAccountData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | The user&#39;s ID | [optional] 
**username** | **str** | The username | [optional] 
**user_email** | **str** | The user&#39;s email | [optional] 
**active** | **int** | Indicates if the user is active | [optional] 
**banned** | **int** | Indicates if the user is banned | [optional] 
**balance** | **str** | The user&#39;s balance | [optional] 
**user_phone** | **str** | The user&#39;s phone number | [optional] 
**reply_to** | **str** | The reply-to email address | [optional] 
**delivery_to** | **str** | The delivery-to email address | [optional] 
**user_first_name** | **str** | The user&#39;s first name | [optional] 
**user_last_name** | **str** | The user&#39;s last name | [optional] 
**account** | **int** | The user&#39;s account number | [optional] 
**account_name** | **str** | The name of the user&#39;s account | [optional] 
**account_billing_email** | **str** | The account billing email | [optional] 
**account_billing_mobile** | **str** | The account billing mobile number | [optional] 
**country** | **str** | The user&#39;s country | [optional] 
**default_country_sms** | **str** | The default country for SMS | [optional] 
**auto_recharge** | **int** | Indicates if auto-recharge is enabled | [optional] 
**auto_recharge_amount** | **str** | The auto-recharge amount | [optional] 
**low_credit_amount** | **str** | The low credit amount | [optional] 
**setting_unicode_sms** | **int** | Setting for Unicode SMS | [optional] 
**setting_email_sms_subject** | **int** | Setting for email SMS subject | [optional] 
**setting_fix_sender_id** | **int** | Setting for fixed sender ID | [optional] 
**setting_sms_message_char_limit** | **int** | Setting for SMS message character limit | [optional] 
**old_dashboard** | **int** | Indicates if the user is using the old dashboard | [optional] 
**balance_commission** | **str** | The balance commission | [optional] 
**timezone** | **str** | The user&#39;s timezone | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 
**subaccount** | [**Subaccount**](Subaccount.md) |  | [optional] 

## Example

```python
from clicksend.models.create_reseller_account_data import CreateResellerAccountData

# TODO update the JSON string below
json = "{}"
# create an instance of CreateResellerAccountData from a JSON string
create_reseller_account_data_instance = CreateResellerAccountData.from_json(json)
# print the JSON string representation of the object
print(CreateResellerAccountData.to_json())

# convert the object into a dict
create_reseller_account_data_dict = create_reseller_account_data_instance.to_dict()
# create an instance of CreateResellerAccountData from a dict
create_reseller_account_data_from_dict = CreateResellerAccountData.from_dict(create_reseller_account_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


