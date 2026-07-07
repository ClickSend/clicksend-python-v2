# Contact


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **int** | The unique identifier for the contact. | [optional] 
**list_id** | **int** | The identifier of the list the contact belongs to. | [optional] 
**phone_number** | **str** | The phone number of the contact. | [optional] 
**first_name** | **str** | The first name of the contact. | [optional] 
**last_name** | **str** | The last name of the contact. | [optional] 
**custom_1** | **str** | Custom field 1. | [optional] 
**custom_2** | **str** | Custom field 2. | [optional] 
**custom_3** | **str** | Custom field 3. | [optional] 
**custom_4** | **str** | Custom field 4. | [optional] 
**date_added** | **datetime** | The date when the contact was added. | [optional] 
**date_updated** | **datetime** | The date when the contact was last updated. | [optional] 
**fax_number** | **str** | The fax number of the contact. | [optional] 
**organization_name** | **str** | The organization name of the contact. | [optional] 
**email** | **str** | The email address of the contact. | [optional] 
**address_line_1** | **str** | The address line 1 of the contact. | [optional] 
**address_line_2** | **str** | The address line 2 of the contact. | [optional] 
**address_city** | **str** | The address city of the contact. | [optional] 
**address_state** | **str** | The address state of the contact. | [optional] 
**address_postal_code** | **str** | The address postal code of the contact. | [optional] 
**address_country** | **str** | The address country of the contact. | [optional] 
**list_name** | **str** | The name of the list the contact belongs to. | [optional] 

## Example

```python
from clicksend.models.contact import Contact

# TODO update the JSON string below
json = "{}"
# create an instance of Contact from a JSON string
contact_instance = Contact.from_json(json)
# print the JSON string representation of the object
print(Contact.to_json())

# convert the object into a dict
contact_dict = contact_instance.to_dict()
# create an instance of Contact from a dict
contact_from_dict = Contact.from_dict(contact_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


