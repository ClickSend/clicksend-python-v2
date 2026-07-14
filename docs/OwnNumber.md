# OwnNumber


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** | The unique identifier for the record. | [optional] 
**account_id** | **UUID** | The unique identifier for the account. | [optional] 
**workspace_id** | **UUID** | The unique identifier for the workspace. | [optional] 
**user_id** | **UUID** | The unique identifier for the user. | [optional] 
**phone_number** | **str** | The user&#39;s phone number. | [optional] 
**country** | **str** | The country code of the phone number. | [optional] 
**label** | **str** | A label for the phone number. | [optional] 
**status** | **str** | The status of the phone number. | [optional] 
**verified_timestamp** | **datetime** | The timestamp when the phone number was verified. | [optional] 
**notified_timestamp** | **str** | The timestamp when the user was last notified about this number, if applicable. | [optional] 
**is_nearing_expiration** | **bool** | Indicates whether the phone number verification is nearing its expiration date: - **true:** The verification was completed more than 11 months ago and will expire soon. You should re-verify your phone number to maintain uninterrupted service. - **false:** The verification is still valid and not approaching expiration. | [optional] 
**created_timestamp** | **datetime** | The timestamp when the record was created. | [optional] 
**updated_timestamp** | **datetime** | The timestamp when the record was last updated. | [optional] 

## Example

```python
from clicksend.models.own_number import OwnNumber

# TODO update the JSON string below
json = "{}"
# create an instance of OwnNumber from a JSON string
own_number_instance = OwnNumber.from_json(json)
# print the JSON string representation of the object
print(OwnNumber.to_json())

# convert the object into a dict
own_number_dict = own_number_instance.to_dict()
# create an instance of OwnNumber from a dict
own_number_from_dict = OwnNumber.from_dict(own_number_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


