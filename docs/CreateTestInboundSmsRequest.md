# CreateTestInboundSmsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | The webhook URL where the inbound SMS will be sent to.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;You can create a webhook URL in &lt;em&gt;Pipedream&lt;/em&gt; to test receiving the inbound SMS. Follow the instructions &lt;a href&#x3D;\&quot;https://help.clicksend.com/en/articles/43703-integration-guide-pipedream\&quot; target&#x3D;\&quot;_blank\&quot;&gt;here.&lt;/a&gt;&lt;/p&gt; &lt;/div&gt;   | 
**webhook_type** | **str** | Specifies the HTTP method used when the webhook sends a request to the URL. The available options are:  - **post** (Default): Sends the event data using an HTTP POST request.      - **get**: Sends the event data as query parameters in an HTTP GET request.      - **json**: Sends the event data using a custom JSON format (via a POST request).      This parameter is used to determine how the data will be transmitted, depending on your preferred method and how the receiving system is designed to process incoming requests. | [optional] 

## Example

```python
from clicksend.models.create_test_inbound_sms_request import CreateTestInboundSmsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTestInboundSmsRequest from a JSON string
create_test_inbound_sms_request_instance = CreateTestInboundSmsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateTestInboundSmsRequest.to_json())

# convert the object into a dict
create_test_inbound_sms_request_dict = create_test_inbound_sms_request_instance.to_dict()
# create an instance of CreateTestInboundSmsRequest from a dict
create_test_inbound_sms_request_from_dict = CreateTestInboundSmsRequest.from_dict(create_test_inbound_sms_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


