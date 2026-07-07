# PostcardRecipient


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | The ID of the user. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount. | [optional] 
**message_id** | **str** | The ID of the message. | [optional] 
**address_name** | **str** | The name associated with the address. | [optional] 
**address_line_1** | **str** | The first line of the address. | [optional] 
**address_line_2** | **str** | The second line of the address. | [optional] 
**address_city** | **str** | The city of the address. | [optional] 
**address_state** | **str** | The state of the address. | [optional] 
**address_postal_code** | **str** | The postal code of the address. | [optional] 
**address_country** | **str** | The country code of the address. | [optional] 
**return_address_id** | **int** | The ID of the return address. | [optional] 
**letter_file_name** | **str** | The filename of the letter file. | [optional] 
**schedule** | **int** | The schedule timestamp of the message. | [optional] 
**ip_address** | **str** | The IP address associated with the message. | [optional] 
**source** | **str** | The source of the message. | [optional] 
**post_price** | **int** | The price of posting the message. | [optional] 
**priority** | **int** | The priority of the message. | [optional] 
**status** | **str** | The status of the message. | [optional] 
**date_added** | **int** | The timestamp when the message was added. | [optional] 
**file_url** | **str** | The URL of the file associated with the message. | [optional] 
**return_address** | [**PostcardRecipientReturnAddress**](PostcardRecipientReturnAddress.md) |  | [optional] 
**api_username** | **str** | The API username associated with the message. | [optional] 

## Example

```python
from clicksend.models.postcard_recipient import PostcardRecipient

# TODO update the JSON string below
json = "{}"
# create an instance of PostcardRecipient from a JSON string
postcard_recipient_instance = PostcardRecipient.from_json(json)
# print the JSON string representation of the object
print(PostcardRecipient.to_json())

# convert the object into a dict
postcard_recipient_dict = postcard_recipient_instance.to_dict()
# create an instance of PostcardRecipient from a dict
postcard_recipient_from_dict = PostcardRecipient.from_dict(postcard_recipient_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


