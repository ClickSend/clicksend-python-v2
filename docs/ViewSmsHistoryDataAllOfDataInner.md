# ViewSmsHistoryDataAllOfDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**direction** | **str** | It can either be in or out:   - **in** - You received a message. it has to do with inbound messages.   - **out** - You are sending a message. It has to do with outbound messages. | [optional] 
**var_date** | **int** | The date you sent the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**to** | **str** | The phone number of the recipient. It should be in &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/E.164\&quot; target&#x3D;\&quot;_blank\&quot;&gt;E.164 format&lt;/a&gt;. | [optional] 
**body** | **str** | The message sent. | [optional] 
**status** | **str** | The status of the SMS. It can either be:  - _Queued_ - _Completed_ - _Scheduled_ - _WaitApproval_ - _Failed_ - _Cancelled_ - _CancelledAfterReview_ - _Received_ - _Sent_  This parameter reflects the actual status of the SMS. It is based on the  status of the SMS sent from the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/SMS_gateway\&quot; target&#x3D;\&quot;_blank\&quot;&gt;SMS gateway&lt;/a&gt;, which is different  from the [API status code](https://developers-dev.clicksend.net/docs/#status-codes). Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**var_from** | **str** | The sender of the message. | [optional] 
**schedule** | **str** | The scheduled date of the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**status_code** | **str** | The status code sent from the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/SMS_gateway\&quot; target&#x3D;\&quot;_blank\&quot;&gt;SMS gateway&lt;/a&gt;. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**status_text** | **str** | A message describing the _status_code_ of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**error_code** | **str** | The error code of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**error_text** | **str** | A message describing the _error_code_ of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**message_id** | **str** | The generated ID of the message. | [optional] 
**message_parts** | **str** | The number of parts the message was broken into. To look at how many parts your message is broken down into, use the &lt;a href&#x3D;\&quot;http://smscharactercount.com/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;&lt;strong&gt;SMS Character Count&lt;/strong&gt;&lt;/a&gt;. | [optional] 
**message_price** | **str** | The price of this message. This depends on the total number of parts of the message. | [optional] 
**from_email** | **str** | The email address to which replies should be emailed to. If omitted, the reply will be emailed back to the user who sent the outgoing SMS | [optional] 
**list_id** | **str** | The _list_id_ of the contact list the message was sent to. This parameter will have a **null** value if you didn’t send to a list in the request. | [optional] 
**custom_string** | **str** | A note that was included with the outgoing SMS. If no note was included, the value is **null**. | [optional] 
**contact_id** | **str** | This is the ID of the contact. This parameter will have a **null** value if you didn’t provide a _contact_id_ in the request. | [optional] 
**user_id** | **int** | The unique user ID of the sender. | [optional] 
**subaccount_id** | **int** | The sub-account of the user. A user can have multiple sub-accounts. | [optional] 
**country** | **str** | The country of the recipient in two-letter format (e.g. US, UK, AU, NZ, etc). | [optional] 
**carrier** | **str** | The phone carrier of the recipient. | [optional] 
**first_name** | **str** | The first name of the recipient. The name will appear if you sent the message to a contact from a contact list. If you are sending directly to a phone number, the value will be **null**. | [optional] 
**last_name** | **str** | The last name of the recipient. The name will appear if you sent the message to a contact from a contact list. If you are sending directly to a phone number, the value will be **null**. | [optional] 
**api_username** | **str** | The username of the SMS sender. This can be a &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/account/subaccounts\&quot; target&#x3D;\&quot;_blank\&quot;&gt;sub-account&lt;/a&gt;. | [optional] 

## Example

```python
from clicksend.models.view_sms_history_data_all_of_data_inner import ViewSmsHistoryDataAllOfDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsHistoryDataAllOfDataInner from a JSON string
view_sms_history_data_all_of_data_inner_instance = ViewSmsHistoryDataAllOfDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewSmsHistoryDataAllOfDataInner.to_json())

# convert the object into a dict
view_sms_history_data_all_of_data_inner_dict = view_sms_history_data_all_of_data_inner_instance.to_dict()
# create an instance of ViewSmsHistoryDataAllOfDataInner from a dict
view_sms_history_data_all_of_data_inner_from_dict = ViewSmsHistoryDataAllOfDataInner.from_dict(view_sms_history_data_all_of_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


