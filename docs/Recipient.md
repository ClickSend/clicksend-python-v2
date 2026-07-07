# Recipient


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
**custom_string** | **str** | A custom string associated with the message. | [optional] 
**schedule** | **int** | The schedule timestamp of the message. | [optional] 
**source** | **str** | The source of the message. | [optional] 
**colour** | **int** | The color setting of the message. | [optional] 
**duplex** | **int** | Whether the message is set to duplex printing. | [optional] 
**post_pages** | **int** | The number of pages in the postal message. | [optional] 
**post_price** | **str** | The price of the postal message. | [optional] 
**priority_post** | **int** | Whether the postal message is set to priority. | [optional] 
**date_added** | **int** | The timestamp when the message was added. | [optional] 
**status** | **str** | The status of the message. | [optional] 
**file_url** | **str** | The URL of the file associated with the message. | [optional] 
**return_address** | [**PostcardRecipientReturnAddress**](PostcardRecipientReturnAddress.md) |  | [optional] 
**api_username** | **str** | The API username associated with the message. | [optional] 

## Example

```python
from clicksend.models.recipient import Recipient

# TODO update the JSON string below
json = "{}"
# create an instance of Recipient from a JSON string
recipient_instance = Recipient.from_json(json)
# print the JSON string representation of the object
print(Recipient.to_json())

# convert the object into a dict
recipient_dict = recipient_instance.to_dict()
# create an instance of Recipient from a dict
recipient_from_dict = Recipient.from_dict(recipient_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


