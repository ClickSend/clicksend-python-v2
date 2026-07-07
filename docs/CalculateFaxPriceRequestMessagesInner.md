# CalculateFaxPriceRequestMessagesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | **str** |  | [optional] 
**var_from** | **str** |  | [optional] 
**to** | **str** |  | [optional] 
**from_email** | **str** |  | [optional] 
**schedule** | **str** |  | [optional] 
**custom_string** | **str** |  | [optional] 

## Example

```python
from clicksend.models.calculate_fax_price_request_messages_inner import CalculateFaxPriceRequestMessagesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateFaxPriceRequestMessagesInner from a JSON string
calculate_fax_price_request_messages_inner_instance = CalculateFaxPriceRequestMessagesInner.from_json(json)
# print the JSON string representation of the object
print(CalculateFaxPriceRequestMessagesInner.to_json())

# convert the object into a dict
calculate_fax_price_request_messages_inner_dict = calculate_fax_price_request_messages_inner_instance.to_dict()
# create an instance of CalculateFaxPriceRequestMessagesInner from a dict
calculate_fax_price_request_messages_inner_from_dict = CalculateFaxPriceRequestMessagesInner.from_dict(calculate_fax_price_request_messages_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


