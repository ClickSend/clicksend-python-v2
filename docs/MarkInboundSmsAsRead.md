# MarkInboundSmsAsRead


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **object** | The parameters related to the inbound SMS.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return &lt;strong&gt;null&lt;/strong/&gt;.&lt;/p&gt; &lt;/div&gt; | [optional] 

## Example

```python
from clicksend.models.mark_inbound_sms_as_read import MarkInboundSmsAsRead

# TODO update the JSON string below
json = "{}"
# create an instance of MarkInboundSmsAsRead from a JSON string
mark_inbound_sms_as_read_instance = MarkInboundSmsAsRead.from_json(json)
# print the JSON string representation of the object
print(MarkInboundSmsAsRead.to_json())

# convert the object into a dict
mark_inbound_sms_as_read_dict = mark_inbound_sms_as_read_instance.to_dict()
# create an instance of MarkInboundSmsAsRead from a dict
mark_inbound_sms_as_read_from_dict = MarkInboundSmsAsRead.from_dict(mark_inbound_sms_as_read_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


