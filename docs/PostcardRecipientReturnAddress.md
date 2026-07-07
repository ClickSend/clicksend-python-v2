# PostcardRecipientReturnAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**return_address_id** | **int** | The ID of the return address. | [optional] 
**user_id** | **int** | The ID of the user associated with the return address. | [optional] 
**address_name** | **str** | The name associated with the return address. | [optional] 
**address_line_1** | **str** | The first line of the return address. | [optional] 
**address_line_2** | **str** | The second line of the return address. | [optional] 
**address_city** | **str** | The city of the return address. | [optional] 
**address_state** | **str** | The state of the return address. | [optional] 
**address_postal_code** | **str** | The postal code of the return address. | [optional] 
**address_country** | **str** | The country code of the return address. | [optional] 

## Example

```python
from clicksend.models.postcard_recipient_return_address import PostcardRecipientReturnAddress

# TODO update the JSON string below
json = "{}"
# create an instance of PostcardRecipientReturnAddress from a JSON string
postcard_recipient_return_address_instance = PostcardRecipientReturnAddress.from_json(json)
# print the JSON string representation of the object
print(PostcardRecipientReturnAddress.to_json())

# convert the object into a dict
postcard_recipient_return_address_dict = postcard_recipient_return_address_instance.to_dict()
# create an instance of PostcardRecipientReturnAddress from a dict
postcard_recipient_return_address_from_dict = PostcardRecipientReturnAddress.from_dict(postcard_recipient_return_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


