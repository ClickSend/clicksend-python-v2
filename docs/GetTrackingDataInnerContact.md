# GetTrackingDataInnerContact


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** | Contact ID of the recipient. Null if the recipient is not a contact. | [optional] 
**first_name** | **str** | First name of the recipient. Null if the recipient has no data for first name. | [optional] 
**last_name** | **str** | Last name of the recipient. Null if the recipient has no data last name. | [optional] 
**phone_number** | **str** | Phone number of the recipient | [optional] 

## Example

```python
from clicksend.models.get_tracking_data_inner_contact import GetTrackingDataInnerContact

# TODO update the JSON string below
json = "{}"
# create an instance of GetTrackingDataInnerContact from a JSON string
get_tracking_data_inner_contact_instance = GetTrackingDataInnerContact.from_json(json)
# print the JSON string representation of the object
print(GetTrackingDataInnerContact.to_json())

# convert the object into a dict
get_tracking_data_inner_contact_dict = get_tracking_data_inner_contact_instance.to_dict()
# create an instance of GetTrackingDataInnerContact from a dict
get_tracking_data_inner_contact_from_dict = GetTrackingDataInnerContact.from_dict(get_tracking_data_inner_contact_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


