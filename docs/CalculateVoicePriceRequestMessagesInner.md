# CalculateVoicePriceRequestMessagesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**to** | **str** |  | [optional] 
**voice** | **str** |  | [optional] 
**lang** | **str** |  | [optional] 
**schedule** | **str** |  | [optional] 
**custom_string** | **str** |  | [optional] 
**asdasd** | **str** |  | [optional] 
**machine_detection** | **int** |  | [optional] 

## Example

```python
from clicksend.models.calculate_voice_price_request_messages_inner import CalculateVoicePriceRequestMessagesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateVoicePriceRequestMessagesInner from a JSON string
calculate_voice_price_request_messages_inner_instance = CalculateVoicePriceRequestMessagesInner.from_json(json)
# print the JSON string representation of the object
print(CalculateVoicePriceRequestMessagesInner.to_json())

# convert the object into a dict
calculate_voice_price_request_messages_inner_dict = calculate_voice_price_request_messages_inner_instance.to_dict()
# create an instance of CalculateVoicePriceRequestMessagesInner from a dict
calculate_voice_price_request_messages_inner_from_dict = CalculateVoicePriceRequestMessagesInner.from_dict(calculate_voice_price_request_messages_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


