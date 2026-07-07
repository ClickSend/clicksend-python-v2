# CalculateMmsPriceRequestMessagesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**body** | **str** |  | [optional] 
**to** | **str** |  | [optional] 
**country** | **str** |  | [optional] 

## Example

```python
from clicksend.models.calculate_mms_price_request_messages_inner import CalculateMmsPriceRequestMessagesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateMmsPriceRequestMessagesInner from a JSON string
calculate_mms_price_request_messages_inner_instance = CalculateMmsPriceRequestMessagesInner.from_json(json)
# print the JSON string representation of the object
print(CalculateMmsPriceRequestMessagesInner.to_json())

# convert the object into a dict
calculate_mms_price_request_messages_inner_dict = calculate_mms_price_request_messages_inner_instance.to_dict()
# create an instance of CalculateMmsPriceRequestMessagesInner from a dict
calculate_mms_price_request_messages_inner_from_dict = CalculateMmsPriceRequestMessagesInner.from_dict(calculate_mms_price_request_messages_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


