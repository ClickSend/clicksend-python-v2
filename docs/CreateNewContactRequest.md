# CreateNewContactRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**phone_number** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**custom_1** | **str** |  | [optional] 
**custom_2** | **str** |  | [optional] 
**custom_3** | **str** |  | [optional] 
**custom_4** | **str** |  | [optional] 
**date_added** | **str** |  | [optional] 
**fax_number** | **str** |  | [optional] 
**organization_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**address_line_1** | **str** |  | [optional] 
**address_line_2** | **str** |  | [optional] 
**address_city** | **str** |  | [optional] 
**address_state** | **str** |  | [optional] 
**address_postal_code** | **str** |  | [optional] 
**address_country** | **str** |  | [optional] 

## Example

```python
from clicksend.models.create_new_contact_request import CreateNewContactRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateNewContactRequest from a JSON string
create_new_contact_request_instance = CreateNewContactRequest.from_json(json)
# print the JSON string representation of the object
print(CreateNewContactRequest.to_json())

# convert the object into a dict
create_new_contact_request_dict = create_new_contact_request_instance.to_dict()
# create an instance of CreateNewContactRequest from a dict
create_new_contact_request_from_dict = CreateNewContactRequest.from_dict(create_new_contact_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


