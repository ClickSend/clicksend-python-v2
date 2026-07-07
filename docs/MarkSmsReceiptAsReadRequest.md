# MarkSmsReceiptAsReadRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**date_before** | **int** | The cutoff date. Receipts sent before this time will be marked as read. It’s in the &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 

## Example

```python
from clicksend.models.mark_sms_receipt_as_read_request import MarkSmsReceiptAsReadRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MarkSmsReceiptAsReadRequest from a JSON string
mark_sms_receipt_as_read_request_instance = MarkSmsReceiptAsReadRequest.from_json(json)
# print the JSON string representation of the object
print(MarkSmsReceiptAsReadRequest.to_json())

# convert the object into a dict
mark_sms_receipt_as_read_request_dict = mark_sms_receipt_as_read_request_instance.to_dict()
# create an instance of MarkSmsReceiptAsReadRequest from a dict
mark_sms_receipt_as_read_request_from_dict = MarkSmsReceiptAsReadRequest.from_dict(mark_sms_receipt_as_read_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


