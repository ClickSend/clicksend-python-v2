# SendLetterRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_url** | **str** |  | [optional] 
**template_used** | **int** |  | [optional] 
**colour** | **int** |  | [optional] 
**duplex** | **int** |  | [optional] 
**recipients** | [**List[SendPostcardRequestRecipientsInner]**](SendPostcardRequestRecipientsInner.md) |  | [optional] 

## Example

```python
from clicksend.models.send_letter_request import SendLetterRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendLetterRequest from a JSON string
send_letter_request_instance = SendLetterRequest.from_json(json)
# print the JSON string representation of the object
print(SendLetterRequest.to_json())

# convert the object into a dict
send_letter_request_dict = send_letter_request_instance.to_dict()
# create an instance of SendLetterRequest from a dict
send_letter_request_from_dict = SendLetterRequest.from_dict(send_letter_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


