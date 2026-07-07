# CreateTestSmsReceiptRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | The webhook URL where the delivery receipt will be sent to. You can set the value to **poll** to send it to the ClickSend   system, and then retrieve it with the **View SMS Receipt** endpoint  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;You can create a webhook URL in Pipedream to test receiving the SMS receipt. Follow the instructions &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://help.clicksend.com/en/articles/43703-integration-guide-pipedream\&quot;&gt;here&lt;/a&gt;.&lt;/p&gt; &lt;/div&gt; | 

## Example

```python
from clicksend.models.create_test_sms_receipt_request import CreateTestSmsReceiptRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTestSmsReceiptRequest from a JSON string
create_test_sms_receipt_request_instance = CreateTestSmsReceiptRequest.from_json(json)
# print the JSON string representation of the object
print(CreateTestSmsReceiptRequest.to_json())

# convert the object into a dict
create_test_sms_receipt_request_dict = create_test_sms_receipt_request_instance.to_dict()
# create an instance of CreateTestSmsReceiptRequest from a dict
create_test_sms_receipt_request_from_dict = CreateTestSmsReceiptRequest.from_dict(create_test_sms_receipt_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


