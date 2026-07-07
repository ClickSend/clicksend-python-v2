# Subaccount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subaccount_id** | **int** | The unique identifier for the subaccount. | [optional] 
**api_username** | **str** | The API username of the subaccount. | [optional] 
**email** | **str** | The email address of the subaccount. | [optional] 
**phone_number** | **str** | The phone number of the subaccount. | [optional] 
**first_name** | **str** | The first name of the subaccount. | [optional] 
**last_name** | **str** | The last name of the subaccount. | [optional] 
**api_key** | **str** | The API key of the subaccount. | [optional] 
**access_users** | **int** | Flag indicating if the subaccount has access to users. | [optional] 
**access_billing** | **int** | Flag indicating if the subaccount has access to billing. | [optional] 
**access_reporting** | **int** | Flag indicating if the subaccount has access to reporting. | [optional] 
**access_contacts** | **int** | Flag indicating if the subaccount has access to contacts. | [optional] 
**access_settings** | **int** | Flag indicating if the subaccount has access to settings. | [optional] 
**access_sms** | **int** | Flag indicating if the subaccount has access to SMS. | [optional] 
**access_email** | **int** | Flag indicating if the subaccount has access to email. | [optional] 
**access_voice** | **int** | Flag indicating if the subaccount has access to voice services. | [optional] 
**access_fax** | **int** | Flag indicating if the subaccount has access to fax services. | [optional] 
**access_post** | **int** | Flag indicating if the subaccount has access to post services. | [optional] 
**access_reseller** | **int** | Flag indicating if the subaccount has access to reseller services. | [optional] 
**access_mms** | **int** | Flag indicating if the subaccount has access to MMS services. | [optional] 
**share_campaigns** | **int** | Flag indicating if the subaccount can share campaigns. | [optional] 
**notes** | **str** | Additional notes for the subaccount. | [optional] 

## Example

```python
from clicksend.models.subaccount import Subaccount

# TODO update the JSON string below
json = "{}"
# create an instance of Subaccount from a JSON string
subaccount_instance = Subaccount.from_json(json)
# print the JSON string representation of the object
print(Subaccount.to_json())

# convert the object into a dict
subaccount_dict = subaccount_instance.to_dict()
# create an instance of Subaccount from a dict
subaccount_from_dict = Subaccount.from_dict(subaccount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


