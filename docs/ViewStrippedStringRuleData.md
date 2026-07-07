# ViewStrippedStringRuleData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule_id** | **int** | The rule id | [optional] 
**stripped_string** | **str** | The string to be stripped | [optional] 

## Example

```python
from clicksend.models.view_stripped_string_rule_data import ViewStrippedStringRuleData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewStrippedStringRuleData from a JSON string
view_stripped_string_rule_data_instance = ViewStrippedStringRuleData.from_json(json)
# print the JSON string representation of the object
print(ViewStrippedStringRuleData.to_json())

# convert the object into a dict
view_stripped_string_rule_data_dict = view_stripped_string_rule_data_instance.to_dict()
# create an instance of ViewStrippedStringRuleData from a dict
view_stripped_string_rule_data_from_dict = ViewStrippedStringRuleData.from_dict(view_stripped_string_rule_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


