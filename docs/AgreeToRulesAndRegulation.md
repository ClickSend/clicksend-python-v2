# AgreeToRulesAndRegulation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**List[GlobalSending]**](GlobalSending.md) |  | [optional] 

## Example

```python
from clicksend.models.agree_to_rules_and_regulation import AgreeToRulesAndRegulation

# TODO update the JSON string below
json = "{}"
# create an instance of AgreeToRulesAndRegulation from a JSON string
agree_to_rules_and_regulation_instance = AgreeToRulesAndRegulation.from_json(json)
# print the JSON string representation of the object
print(AgreeToRulesAndRegulation.to_json())

# convert the object into a dict
agree_to_rules_and_regulation_dict = agree_to_rules_and_regulation_instance.to_dict()
# create an instance of AgreeToRulesAndRegulation from a dict
agree_to_rules_and_regulation_from_dict = AgreeToRulesAndRegulation.from_dict(agree_to_rules_and_regulation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


