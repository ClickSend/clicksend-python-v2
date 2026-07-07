# SendFaxRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_url** | **str** |  | [optional] 
**messages** | [**List[SendFaxRequestMessagesInner]**](SendFaxRequestMessagesInner.md) |  | [optional] 

## Example

```python
from clicksend.models.send_fax_request import SendFaxRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendFaxRequest from a JSON string
send_fax_request_instance = SendFaxRequest.from_json(json)
# print the JSON string representation of the object
print(SendFaxRequest.to_json())

# convert the object into a dict
send_fax_request_dict = send_fax_request_instance.to_dict()
# create an instance of SendFaxRequest from a dict
send_fax_request_from_dict = SendFaxRequest.from_dict(send_fax_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


