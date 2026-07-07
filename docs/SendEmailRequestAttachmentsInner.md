# SendEmailRequestAttachmentsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**filename** | **str** |  | [optional] 
**disposition** | **str** |  | [optional] 
**content_id** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_email_request_attachments_inner import SendEmailRequestAttachmentsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailRequestAttachmentsInner from a JSON string
send_email_request_attachments_inner_instance = SendEmailRequestAttachmentsInner.from_json(json)
# print the JSON string representation of the object
print(SendEmailRequestAttachmentsInner.to_json())

# convert the object into a dict
send_email_request_attachments_inner_dict = send_email_request_attachments_inner_instance.to_dict()
# create an instance of SendEmailRequestAttachmentsInner from a dict
send_email_request_attachments_inner_from_dict = SendEmailRequestAttachmentsInner.from_dict(send_email_request_attachments_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


