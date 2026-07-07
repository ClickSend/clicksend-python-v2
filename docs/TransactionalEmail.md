# TransactionalEmail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | The ID of the user. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount. | [optional] 
**from_email_address_id** | **int** | The ID of the from email address. | [optional] 
**from_name** | **str** | The name of the sender. | [optional] 
**to** | [**List[SendEmailRequestToInner]**](SendEmailRequestToInner.md) |  | [optional] 
**cc** | [**List[SendEmailRequestToInner]**](SendEmailRequestToInner.md) |  | [optional] 
**bcc** | [**List[SendEmailRequestToInner]**](SendEmailRequestToInner.md) |  | [optional] 
**subject** | **str** | The subject of the email. | [optional] 
**body** | **str** | The HTML body of the email. | [optional] 
**body_plain_text** | **str** | The plain text body of the email. | [optional] 
**schedule** | **int** | The timestamp indicating the scheduled time of the email. | [optional] 
**message_id** | **str** | The ID of the email message. | [optional] 
**status** | **str** | The status of the email. | [optional] 
**status_text** | **str** | The text description of the email status. | [optional] 
**soft_bounce_count** | **int** | The count of soft bounces. | [optional] 
**hard_bounce_count** | **int** | The count of hard bounces. | [optional] 
**price** | **str** | The price of the email. | [optional] 
**date_added** | **int** | The timestamp indicating when the email was added. | [optional] 
**custom_string** | **str** | A custom string. | [optional] 
**attachments** | [**List[Attachment]**](Attachment.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.transactional_email import TransactionalEmail

# TODO update the JSON string below
json = "{}"
# create an instance of TransactionalEmail from a JSON string
transactional_email_instance = TransactionalEmail.from_json(json)
# print the JSON string representation of the object
print(TransactionalEmail.to_json())

# convert the object into a dict
transactional_email_dict = transactional_email_instance.to_dict()
# create an instance of TransactionalEmail from a dict
transactional_email_from_dict = TransactionalEmail.from_dict(transactional_email_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


