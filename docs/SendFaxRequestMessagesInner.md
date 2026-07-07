# SendFaxRequestMessagesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**to** | **str** |  | [optional] 
**custom_string** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_fax_request_messages_inner import SendFaxRequestMessagesInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendFaxRequestMessagesInner from a JSON string
send_fax_request_messages_inner_instance = SendFaxRequestMessagesInner.from_json(json)
# print the JSON string representation of the object
print(SendFaxRequestMessagesInner.to_json())

# convert the object into a dict
send_fax_request_messages_inner_dict = send_fax_request_messages_inner_instance.to_dict()
# create an instance of SendFaxRequestMessagesInner from a dict
send_fax_request_messages_inner_from_dict = SendFaxRequestMessagesInner.from_dict(send_fax_request_messages_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


