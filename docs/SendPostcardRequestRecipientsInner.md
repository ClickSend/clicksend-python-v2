# SendPostcardRequestRecipientsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_name** | **str** |  | [optional] 
**address_city** | **str** |  | [optional] 
**address_state** | **str** |  | [optional] 
**address_postal_code** | **str** |  | [optional] 
**address_country** | **str** |  | [optional] 
**address_line_1** | **str** |  | [optional] 
**return_address_id** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_postcard_request_recipients_inner import SendPostcardRequestRecipientsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendPostcardRequestRecipientsInner from a JSON string
send_postcard_request_recipients_inner_instance = SendPostcardRequestRecipientsInner.from_json(json)
# print the JSON string representation of the object
print(SendPostcardRequestRecipientsInner.to_json())

# convert the object into a dict
send_postcard_request_recipients_inner_dict = send_postcard_request_recipients_inner_instance.to_dict()
# create an instance of SendPostcardRequestRecipientsInner from a dict
send_postcard_request_recipients_inner_from_dict = SendPostcardRequestRecipientsInner.from_dict(send_postcard_request_recipients_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


