# GlobalSending


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the country. | [optional] 
**name** | **str** | The name of the country. | [optional] 
**code** | **str** | The country code. | [optional] 
**region** | **str** | The region of the country. | [optional] 
**agreed_at** | **str** | The date when the country was agreed upon. | [optional] 
**registration_entity** | **str** | The entity responsible for the registration. | [optional] 
**registration_status** | [**GlobalSendingRegistrationStatus**](GlobalSendingRegistrationStatus.md) |  | [optional] 
**jotform_id** | **str** | The ID of the country in JotForm. | [optional] 
**sms_registration_type** | **int** | The type of SMS registration. | [optional] 
**block_registration** | **int** | Indicates if registration is blocked. | [optional] 
**block_leads** | **int** | Indicates if leads are blocked. | [optional] 
**trial_from_address** | **str** | The trial from address. | [optional] 
**restricted_sending** | **int** | Indicates if sending is restricted. | [optional] 
**trial_sending** | **int** | Indicates if trial sending is allowed. | [optional] 
**trial_sending_description** | **str** | Description of trial sending. | [optional] 
**has_regulation_requirements** | **int** | Indicates if there are regulation requirements. | [optional] 
**registration_steps_url** | **str** | URL for registration steps. | [optional] 
**regulation_requirements_description** | **str** | Description of regulation requirements. | [optional] 

## Example

```python
from clicksend.models.global_sending import GlobalSending

# TODO update the JSON string below
json = "{}"
# create an instance of GlobalSending from a JSON string
global_sending_instance = GlobalSending.from_json(json)
# print the JSON string representation of the object
print(GlobalSending.to_json())

# convert the object into a dict
global_sending_dict = global_sending_instance.to_dict()
# create an instance of GlobalSending from a dict
global_sending_from_dict = GlobalSending.from_dict(global_sending_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


