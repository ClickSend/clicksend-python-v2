# PurchaseRechargePackageData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | The ID of the user. | [optional] 
**amount** | **int** | The amount of the package. | [optional] 
**currency** | **str** | The currency of the package. | [optional] 
**amount_aud** | **int** | The amount of the package in AUD. | [optional] 
**var_date** | **int** | The timestamp of when the package was purchased. | [optional] 

## Example

```python
from clicksend.models.purchase_recharge_package_data import PurchaseRechargePackageData

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseRechargePackageData from a JSON string
purchase_recharge_package_data_instance = PurchaseRechargePackageData.from_json(json)
# print the JSON string representation of the object
print(PurchaseRechargePackageData.to_json())

# convert the object into a dict
purchase_recharge_package_data_dict = purchase_recharge_package_data_instance.to_dict()
# create an instance of PurchaseRechargePackageData from a dict
purchase_recharge_package_data_from_dict = PurchaseRechargePackageData.from_dict(purchase_recharge_package_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


