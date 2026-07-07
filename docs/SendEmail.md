# SendEmail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**TransactionalEmail**](TransactionalEmail.md) |  | [optional] 

## Example

```python
from clicksend.models.send_email import SendEmail

# TODO update the JSON string below
json = "{}"
# create an instance of SendEmail from a JSON string
send_email_instance = SendEmail.from_json(json)
# print the JSON string representation of the object
print(SendEmail.to_json())

# convert the object into a dict
send_email_dict = send_email_instance.to_dict()
# create an instance of SendEmail from a dict
send_email_from_dict = SendEmail.from_dict(send_email_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


