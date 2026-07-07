# SendMmsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**media_file** | **str** |  | [optional] 
**messages** | [**List[SendMmsRequestMessagesInner]**](SendMmsRequestMessagesInner.md) |  | [optional] 

## Example

```python
from clicksend.models.send_mms_request import SendMmsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendMmsRequest from a JSON string
send_mms_request_instance = SendMmsRequest.from_json(json)
# print the JSON string representation of the object
print(SendMmsRequest.to_json())

# convert the object into a dict
send_mms_request_dict = send_mms_request_instance.to_dict()
# create an instance of SendMmsRequest from a dict
send_mms_request_from_dict = SendMmsRequest.from_dict(send_mms_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


