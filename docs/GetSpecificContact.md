# GetSpecificContact


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**Contact**](Contact.md) |  | [optional] 

## Example

```python
from clicksend.models.get_specific_contact import GetSpecificContact

# TODO update the JSON string below
json = "{}"
# create an instance of GetSpecificContact from a JSON string
get_specific_contact_instance = GetSpecificContact.from_json(json)
# print the JSON string representation of the object
print(GetSpecificContact.to_json())

# convert the object into a dict
get_specific_contact_dict = get_specific_contact_instance.to_dict()
# create an instance of GetSpecificContact from a dict
get_specific_contact_from_dict = GetSpecificContact.from_dict(get_specific_contact_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


