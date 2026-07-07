# CancelSms


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **str** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **object** | The parameters related to the scheduled SMS.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return &lt;strong&gt;null&lt;/strong/&gt;.&lt;/p&gt; &lt;/div&gt; | [optional] 

## Example

```python
from clicksend.models.cancel_sms import CancelSms

# TODO update the JSON string below
json = "{}"
# create an instance of CancelSms from a JSON string
cancel_sms_instance = CancelSms.from_json(json)
# print the JSON string representation of the object
print(CancelSms.to_json())

# convert the object into a dict
cancel_sms_dict = cancel_sms_instance.to_dict()
# create an instance of CancelSms from a dict
cancel_sms_from_dict = CancelSms.from_dict(cancel_sms_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


