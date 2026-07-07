# CreateEmailTemplateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id_master** | **int** |  | [optional] 
**template_name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.create_email_template_request import CreateEmailTemplateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateEmailTemplateRequest from a JSON string
create_email_template_request_instance = CreateEmailTemplateRequest.from_json(json)
# print the JSON string representation of the object
print(CreateEmailTemplateRequest.to_json())

# convert the object into a dict
create_email_template_request_dict = create_email_template_request_instance.to_dict()
# create an instance of CreateEmailTemplateRequest from a dict
create_email_template_request_from_dict = CreateEmailTemplateRequest.from_dict(create_email_template_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


