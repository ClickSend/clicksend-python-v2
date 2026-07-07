# DeleteEmailTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **List[str]** |  | [optional] 

## Example

```python
from clicksend.models.delete_email_template import DeleteEmailTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteEmailTemplate from a JSON string
delete_email_template_instance = DeleteEmailTemplate.from_json(json)
# print the JSON string representation of the object
print(DeleteEmailTemplate.to_json())

# convert the object into a dict
delete_email_template_dict = delete_email_template_instance.to_dict()
# create an instance of DeleteEmailTemplate from a dict
delete_email_template_from_dict = DeleteEmailTemplate.from_dict(delete_email_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


