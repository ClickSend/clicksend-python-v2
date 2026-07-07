# SendPostcardRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_urls** | **List[str]** |  | [optional] 
**recipients** | [**List[SendPostcardRequestRecipientsInner]**](SendPostcardRequestRecipientsInner.md) |  | [optional] 

## Example

```python
from clicksend.models.send_postcard_request import SendPostcardRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendPostcardRequest from a JSON string
send_postcard_request_instance = SendPostcardRequest.from_json(json)
# print the JSON string representation of the object
print(SendPostcardRequest.to_json())

# convert the object into a dict
send_postcard_request_dict = send_postcard_request_instance.to_dict()
# create an instance of SendPostcardRequest from a dict
send_postcard_request_from_dict = SendPostcardRequest.from_dict(send_postcard_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


