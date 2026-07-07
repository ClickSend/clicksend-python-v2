# CreateSubaccountRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_username** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**user_id** | **int** |  | [optional] 
**sms_deidentify_message** | **int** |  | [optional] 
**access_smpp** | **int** |  | [optional] 
**access_users** | **int** |  | [optional] 
**access_billing** | **int** |  | [optional] 
**access_reporting** | **int** |  | [optional] 
**access_contacts** | **int** |  | [optional] 
**access_settings** | **int** |  | [optional] 
**notes** | **str** |  | [optional] 

## Example

```python
from clicksend.models.create_subaccount_request import CreateSubaccountRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSubaccountRequest from a JSON string
create_subaccount_request_instance = CreateSubaccountRequest.from_json(json)
# print the JSON string representation of the object
print(CreateSubaccountRequest.to_json())

# convert the object into a dict
create_subaccount_request_dict = create_subaccount_request_instance.to_dict()
# create an instance of CreateSubaccountRequest from a dict
create_subaccount_request_from_dict = CreateSubaccountRequest.from_dict(create_subaccount_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


