# Fax


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | The ID of the user. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount. | [optional] 
**list_id** | **int** | The ID of the list. | [optional] 
**message_id** | **str** | The ID of the message. | [optional] 
**to** | **str** | The recipient&#39;s phone number. | [optional] 
**var_from** | **str** | The sender&#39;s phone number. | [optional] 
**carrier** | **str** | The carrier associated with the message. | [optional] 
**country** | **str** | The country code. | [optional] 
**custom_string** | **str** | A custom string associated with the message. | [optional] 
**schedule** | **str** | The scheduled time for sending the message. | [optional] 
**message_pages** | **int** | The number of pages in the message. | [optional] 
**message_price** | **str** | The price of the message. | [optional] 
**status_code** | **str** | The status code of the message. | [optional] 
**status_text** | **str** | The status text of the message. | [optional] 
**date_added** | **int** | The date when the message was added. | [optional] 
**from_email** | **str** | The sender&#39;s email address. | [optional] 
**file_url** | **str** | The URL of the file associated with the message. | [optional] 
**status** | **str** | The status of the message. | [optional] 

## Example

```python
from clicksend.models.fax import Fax

# TODO update the JSON string below
json = "{}"
# create an instance of Fax from a JSON string
fax_instance = Fax.from_json(json)
# print the JSON string representation of the object
print(Fax.to_json())

# convert the object into a dict
fax_dict = fax_instance.to_dict()
# create an instance of Fax from a dict
fax_from_dict = Fax.from_dict(fax_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


