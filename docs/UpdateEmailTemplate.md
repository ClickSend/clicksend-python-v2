# UpdateEmailTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**UserEmailTemplate**](UserEmailTemplate.md) |  | [optional] 

## Example

```python
from clicksend.models.update_email_template import UpdateEmailTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateEmailTemplate from a JSON string
update_email_template_instance = UpdateEmailTemplate.from_json(json)
# print the JSON string representation of the object
print(UpdateEmailTemplate.to_json())

# convert the object into a dict
update_email_template_dict = update_email_template_instance.to_dict()
# create an instance of UpdateEmailTemplate from a dict
update_email_template_from_dict = UpdateEmailTemplate.from_dict(update_email_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


