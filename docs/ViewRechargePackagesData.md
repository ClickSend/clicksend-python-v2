# ViewRechargePackagesData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**packages** | [**List[ViewRechargePackagesDataPackagesInner]**](ViewRechargePackagesDataPackagesInner.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.view_recharge_packages_data import ViewRechargePackagesData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewRechargePackagesData from a JSON string
view_recharge_packages_data_instance = ViewRechargePackagesData.from_json(json)
# print the JSON string representation of the object
print(ViewRechargePackagesData.to_json())

# convert the object into a dict
view_recharge_packages_data_dict = view_recharge_packages_data_instance.to_dict()
# create an instance of ViewRechargePackagesData from a dict
view_recharge_packages_data_from_dict = ViewRechargePackagesData.from_dict(view_recharge_packages_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


