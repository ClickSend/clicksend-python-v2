# DeliveryIssue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**issue_id** | **str** | The unique identifier of the delivery issue. | [optional] 
**user_id** | **int** | The unique identifier of the user. | [optional] 
**message_id** | **str** | The message id of the message. | [optional] 
**type** | **str** | The type of message, must be one of the following values SMS, MMS, VOICE, EMAIL_MARKETING, EMAIL_TRANSACTIONAL, FAX, POST. | [optional] 
**description** | **str** | The description of the message. | [optional] 
**client_comments** | **str** | The user&#39;s comments. | [optional] 
**support_comments** | **str** | The support&#39;s comments. | [optional] 
**status** | **str** | The status of the delivery issue. | [optional] 
**date_added** | **float** | The date and time the delivery issue was created. | [optional] 
**resolved** | **float** | Flag indicating if the delivery issue is resolved. | [optional] 
**email_address** | **str** | The user&#39;s email address. | [optional] 

## Example

```python
from clicksend.models.delivery_issue import DeliveryIssue

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryIssue from a JSON string
delivery_issue_instance = DeliveryIssue.from_json(json)
# print the JSON string representation of the object
print(DeliveryIssue.to_json())

# convert the object into a dict
delivery_issue_dict = delivery_issue_instance.to_dict()
# create an instance of DeliveryIssue from a dict
delivery_issue_from_dict = DeliveryIssue.from_dict(delivery_issue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


