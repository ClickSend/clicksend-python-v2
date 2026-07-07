# PurchaseDedicatedNumberData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dedicated_number** | **str** | The new dedicated number. | [optional] 
**country** | **str** | The country code of the new dedicated number. | [optional] 
**price_total** | **str** | The total price of the new dedicated number. | [optional] 
**price_setup** | **str** | The setup price of the new dedicated number. | [optional] 
**price_monthly** | **str** | The monthly price of the new dedicated number. | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.purchase_dedicated_number_data import PurchaseDedicatedNumberData

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseDedicatedNumberData from a JSON string
purchase_dedicated_number_data_instance = PurchaseDedicatedNumberData.from_json(json)
# print the JSON string representation of the object
print(PurchaseDedicatedNumberData.to_json())

# convert the object into a dict
purchase_dedicated_number_data_dict = purchase_dedicated_number_data_instance.to_dict()
# create an instance of PurchaseDedicatedNumberData from a dict
purchase_dedicated_number_data_from_dict = PurchaseDedicatedNumberData.from_dict(purchase_dedicated_number_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


