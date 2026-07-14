# Currency

The parameters related to currency.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency_name_short** | **str** | The currency used for the sender in three-letter format (e.g. USD, EUR, AUD, NZD, etc). | [optional] 
**currency_prefix_d** | **str** | The symbol used to indicate the currency of the sender (e.g. $ , €, etc). | [optional] 
**currency_prefix_c** | **str** | The currency basic unit (e.g. cents). | [optional] 
**currency_name_long** | **str** | The full name of the currency. | [optional] 
**min_recharge_amount** | **str** | The minimum amount that can be used to recharge the account, in this currency. | [optional] 
**max_recharge_amount** | **str** | The maximum amount that can be used to recharge the account, in this currency. | [optional] 

## Example

```python
from clicksend.models.currency import Currency

# TODO update the JSON string below
json = "{}"
# create an instance of Currency from a JSON string
currency_instance = Currency.from_json(json)
# print the JSON string representation of the object
print(Currency.to_json())

# convert the object into a dict
currency_dict = currency_instance.to_dict()
# create an instance of Currency from a dict
currency_from_dict = Currency.from_dict(currency_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


