# UpdateStrippedStringRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewStrippedStringRuleData**](ViewStrippedStringRuleData.md) |  | [optional] 

## Example

```python
from clicksend.models.update_stripped_string_rule import UpdateStrippedStringRule

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateStrippedStringRule from a JSON string
update_stripped_string_rule_instance = UpdateStrippedStringRule.from_json(json)
# print the JSON string representation of the object
print(UpdateStrippedStringRule.to_json())

# convert the object into a dict
update_stripped_string_rule_dict = update_stripped_string_rule_instance.to_dict()
# create an instance of UpdateStrippedStringRule from a dict
update_stripped_string_rule_from_dict = UpdateStrippedStringRule.from_dict(update_stripped_string_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


