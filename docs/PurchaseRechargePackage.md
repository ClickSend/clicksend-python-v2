# PurchaseRechargePackage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**PurchaseRechargePackageData**](PurchaseRechargePackageData.md) |  | [optional] 

## Example

```python
from clicksend.models.purchase_recharge_package import PurchaseRechargePackage

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseRechargePackage from a JSON string
purchase_recharge_package_instance = PurchaseRechargePackage.from_json(json)
# print the JSON string representation of the object
print(PurchaseRechargePackage.to_json())

# convert the object into a dict
purchase_recharge_package_dict = purchase_recharge_package_instance.to_dict()
# create an instance of PurchaseRechargePackage from a dict
purchase_recharge_package_from_dict = PurchaseRechargePackage.from_dict(purchase_recharge_package_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


