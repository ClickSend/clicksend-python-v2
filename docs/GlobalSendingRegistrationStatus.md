# GlobalSendingRegistrationStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the registration status. | [optional] 
**name** | **str** | The name of the registration status. | [optional] 

## Example

```python
from clicksend.models.global_sending_registration_status import GlobalSendingRegistrationStatus

# TODO update the JSON string below
json = "{}"
# create an instance of GlobalSendingRegistrationStatus from a JSON string
global_sending_registration_status_instance = GlobalSendingRegistrationStatus.from_json(json)
# print the JSON string representation of the object
print(GlobalSendingRegistrationStatus.to_json())

# convert the object into a dict
global_sending_registration_status_dict = global_sending_registration_status_instance.to_dict()
# create an instance of GlobalSendingRegistrationStatus from a dict
global_sending_registration_status_from_dict = GlobalSendingRegistrationStatus.from_dict(global_sending_registration_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


