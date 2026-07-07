# SendEmailRequestToInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_email_request_to_inner import SendEmailRequestToInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailRequestToInner from a JSON string
send_email_request_to_inner_instance = SendEmailRequestToInner.from_json(json)
# print the JSON string representation of the object
print(SendEmailRequestToInner.to_json())

# convert the object into a dict
send_email_request_to_inner_dict = send_email_request_to_inner_instance.to_dict()
# create an instance of SendEmailRequestToInner from a dict
send_email_request_to_inner_from_dict = SendEmailRequestToInner.from_dict(send_email_request_to_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


