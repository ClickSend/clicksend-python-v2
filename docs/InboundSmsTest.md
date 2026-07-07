# InboundSmsTest

The parameters related to the message receipt.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp_send** | **int** | The time you sent the test message. It’s in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format.&lt;/a&gt; | [optional] 
**var_from** | **str** | This is a random number used for testing purposes. | [optional] 
**body** | **str** | The sample test message. | [optional] 
**original_body** | **str** | The sample test message you sent to your recipient. | [optional] 
**original_message_id** | **str** | The generated ID of the message that you sent to your receipient.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This &lt;em&gt;original_message_id&lt;/em&gt; is different from the ID that is generated when sending an actual SMS. This ID is used for testing only.&lt;/p&gt; &lt;/div&gt; | [optional] 
**to** | **str** | The receiver of the inbound message, which can be either the shared number or the dedicated number you used to send the message. | [optional] 
**custom_string** | **str** | The sample test note that was included with the inbound SMS. | [optional] 
**message_id** | **str** | The generated ID of the inbound SMS. This ID is typically used as a reference for &lt;a href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;customer support&lt;/a&gt; in case of any issues. | [optional] 
**keyword** | **str** | The keyword of the inbound SMS.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return &lt;strong&gt;null.&lt;/strong&gt;&lt;/p&gt; &lt;/div&gt; | [optional] 

## Example

```python
from clicksend.models.inbound_sms_test import InboundSmsTest

# TODO update the JSON string below
json = "{}"
# create an instance of InboundSmsTest from a JSON string
inbound_sms_test_instance = InboundSmsTest.from_json(json)
# print the JSON string representation of the object
print(InboundSmsTest.to_json())

# convert the object into a dict
inbound_sms_test_dict = inbound_sms_test_instance.to_dict()
# create an instance of InboundSmsTest from a dict
inbound_sms_test_from_dict = InboundSmsTest.from_dict(inbound_sms_test_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


