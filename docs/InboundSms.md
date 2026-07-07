# InboundSms

The parameters related to the message receipt.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp** | **int** | The time you receive the inbound message.. It’s in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format.&lt;/a&gt; | [optional] 
**var_from** | **str** | The sender of the message, which is the phone number of the recipient who replied to you. Your recipient can’t reply to an alpha tag (business name). | [optional] 
**body** | **str** | The message you received from your recipient. | [optional] 
**original_body** | **str** | The last message you sent to your recipient. | [optional] 
**original_message_id** | **str** | The generated ID of the message that you sent to your receipient. | [optional] 
**to** | **str** | The receiver of the inbound message, which can be either the shared number or the dedicated number you used to send the message. | [optional] 
**custom_string** | **str** | A note that was included with the inbound SMS. If no note was included, the value will be an empty string. | [optional] 
**message_id** | **str** | The generated ID of the inbound SMS. This ID is typically used as a reference for &lt;a href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;customer support&lt;/a&gt; in case of any issues. | [optional] 
**keyword** | **str** | The keyword of the inbound SMS.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return the first word of the body message.&lt;/p&gt; &lt;/div&gt; | [optional] 

## Example

```python
from clicksend.models.inbound_sms import InboundSms

# TODO update the JSON string below
json = "{}"
# create an instance of InboundSms from a JSON string
inbound_sms_instance = InboundSms.from_json(json)
# print the JSON string representation of the object
print(InboundSms.to_json())

# convert the object into a dict
inbound_sms_dict = inbound_sms_instance.to_dict()
# create an instance of InboundSms from a dict
inbound_sms_from_dict = InboundSms.from_dict(inbound_sms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


