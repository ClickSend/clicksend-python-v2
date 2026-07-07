# ViewASpecificSmsTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **str** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewASpecificSmsTemplateData**](ViewASpecificSmsTemplateData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_a_specific_sms_template import ViewASpecificSmsTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of ViewASpecificSmsTemplate from a JSON string
view_a_specific_sms_template_instance = ViewASpecificSmsTemplate.from_json(json)
# print the JSON string representation of the object
print(ViewASpecificSmsTemplate.to_json())

# convert the object into a dict
view_a_specific_sms_template_dict = view_a_specific_sms_template_instance.to_dict()
# create an instance of ViewASpecificSmsTemplate from a dict
view_a_specific_sms_template_from_dict = ViewASpecificSmsTemplate.from_dict(view_a_specific_sms_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


