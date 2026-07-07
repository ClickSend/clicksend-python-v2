# CreateStrippedStringRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewStrippedStringRulesDataDataInner**](ViewStrippedStringRulesDataDataInner.md) |  | [optional] 

## Example

```python
from clicksend.models.create_stripped_string_rule import CreateStrippedStringRule

# TODO update the JSON string below
json = "{}"
# create an instance of CreateStrippedStringRule from a JSON string
create_stripped_string_rule_instance = CreateStrippedStringRule.from_json(json)
# print the JSON string representation of the object
print(CreateStrippedStringRule.to_json())

# convert the object into a dict
create_stripped_string_rule_dict = create_stripped_string_rule_instance.to_dict()
# create an instance of CreateStrippedStringRule from a dict
create_stripped_string_rule_from_dict = CreateStrippedStringRule.from_dict(create_stripped_string_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


