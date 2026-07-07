# CreateSmsTemplateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_name** | **str** | The name of the template. | [optional] 
**body** | **str** | body String The main content of your template. | [optional] 

## Example

```python
from clicksend.models.create_sms_template_request import CreateSmsTemplateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSmsTemplateRequest from a JSON string
create_sms_template_request_instance = CreateSmsTemplateRequest.from_json(json)
# print the JSON string representation of the object
print(CreateSmsTemplateRequest.to_json())

# convert the object into a dict
create_sms_template_request_dict = create_sms_template_request_instance.to_dict()
# create an instance of CreateSmsTemplateRequest from a dict
create_sms_template_request_from_dict = CreateSmsTemplateRequest.from_dict(create_sms_template_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


