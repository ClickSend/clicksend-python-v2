# SendMmsRequestMessagesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | **str** |  | [optional] [default to 'sdk']
**to** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**schedule** | **int** |  | [optional] 

## Example

```python
from clicksend.models.send_mms_request_messages_inner import SendMmsRequestMessagesInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendMmsRequestMessagesInner from a JSON string
send_mms_request_messages_inner_instance = SendMmsRequestMessagesInner.from_json(json)
# print the JSON string representation of the object
print(SendMmsRequestMessagesInner.to_json())

# convert the object into a dict
send_mms_request_messages_inner_dict = send_mms_request_messages_inner_instance.to_dict()
# create an instance of SendMmsRequestMessagesInner from a dict
send_mms_request_messages_inner_from_dict = SendMmsRequestMessagesInner.from_dict(send_mms_request_messages_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


