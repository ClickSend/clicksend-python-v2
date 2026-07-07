# DefaultSenderDefaultSenderStrategiesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sender_type** | **str** | Type of the sender. | 
**sender_id** | **str** | Identifier for the sender. Must be between 3-20 characters. | 
**sender_country_code** | **str** | ISO 3166-1 alpha-2 formatted country code. | [optional] 
**priority** | **int** | Priority level of the sender in the strategy. Must be a positive integer. | 
**status** | **str** | Status of the sender in the strategy. | 
**note** | **str** | Note providing additional context about the sender. Maximum length of 200 characters. Optional. | [optional] 

## Example

```python
from clicksend.models.default_sender_default_sender_strategies_inner import DefaultSenderDefaultSenderStrategiesInner

# TODO update the JSON string below
json = "{}"
# create an instance of DefaultSenderDefaultSenderStrategiesInner from a JSON string
default_sender_default_sender_strategies_inner_instance = DefaultSenderDefaultSenderStrategiesInner.from_json(json)
# print the JSON string representation of the object
print(DefaultSenderDefaultSenderStrategiesInner.to_json())

# convert the object into a dict
default_sender_default_sender_strategies_inner_dict = default_sender_default_sender_strategies_inner_instance.to_dict()
# create an instance of DefaultSenderDefaultSenderStrategiesInner from a dict
default_sender_default_sender_strategies_inner_from_dict = DefaultSenderDefaultSenderStrategiesInner.from_dict(default_sender_default_sender_strategies_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


