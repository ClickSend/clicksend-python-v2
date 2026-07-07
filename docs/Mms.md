# Mms


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**list_id** | **str** | The ID of the list (if applicable). | [optional] 
**contact_id** | **int** | The ID of the contact. | [optional] 
**message_id** | **str** | The ID of the message. | [optional] 
**to** | **str** | The recipient of the message. | [optional] 
**subject** | **str** | The subject of the message. | [optional] 
**var_from** | **str** | The sender of the message. | [optional] 
**body** | **str** | The body of the message. | [optional] 
**country** | **str** | The country code. | [optional] 
**custom_string** | **str** | Custom string associated with the message. | [optional] 
**schedule** | **str** | The schedule time of the message. | [optional] 
**message_parts** | **int** | The number of parts the message was split into. | [optional] 
**message_price** | **str** | The price of the message. | [optional] 
**media_file_url** | **str** | The URL of the media file attached to the message. | [optional] 
**status** | **str** | The status of the message. | [optional] 

## Example

```python
from clicksend.models.mms import Mms

# TODO update the JSON string below
json = "{}"
# create an instance of Mms from a JSON string
mms_instance = Mms.from_json(json)
# print the JSON string representation of the object
print(Mms.to_json())

# convert the object into a dict
mms_dict = mms_instance.to_dict()
# create an instance of Mms from a dict
mms_from_dict = Mms.from_dict(mms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


