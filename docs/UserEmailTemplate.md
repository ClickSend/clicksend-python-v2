# UserEmailTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **int** | The unique identifier for the template. | [optional] 
**template_id_master** | **int** | The unique identifier for the template. | [optional] 
**template_name** | **str** | The name of the template. | [optional] 
**body** | **str** | The body of the template. | [optional] 

## Example

```python
from clicksend.models.user_email_template import UserEmailTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of UserEmailTemplate from a JSON string
user_email_template_instance = UserEmailTemplate.from_json(json)
# print the JSON string representation of the object
print(UserEmailTemplate.to_json())

# convert the object into a dict
user_email_template_dict = user_email_template_instance.to_dict()
# create an instance of UserEmailTemplate from a dict
user_email_template_from_dict = UserEmailTemplate.from_dict(user_email_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


