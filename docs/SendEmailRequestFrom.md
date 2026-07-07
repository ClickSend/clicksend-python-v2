# SendEmailRequestFrom


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.send_email_request_from import SendEmailRequestFrom

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmailRequestFrom from a JSON string
send_email_request_from_instance = SendEmailRequestFrom.from_json(json)
# print the JSON string representation of the object
print(SendEmailRequestFrom.to_json())

# convert the object into a dict
send_email_request_from_dict = send_email_request_from_instance.to_dict()
# create an instance of SendEmailRequestFrom from a dict
send_email_request_from_from_dict = SendEmailRequestFrom.from_dict(send_email_request_from_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


