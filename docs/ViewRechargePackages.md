# ViewRechargePackages


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**ViewRechargePackagesData**](ViewRechargePackagesData.md) |  | [optional] 

## Example

```python
from clicksend.models.view_recharge_packages import ViewRechargePackages

# TODO update the JSON string below
json = "{}"
# create an instance of ViewRechargePackages from a JSON string
view_recharge_packages_instance = ViewRechargePackages.from_json(json)
# print the JSON string representation of the object
print(ViewRechargePackages.to_json())

# convert the object into a dict
view_recharge_packages_dict = view_recharge_packages_instance.to_dict()
# create an instance of ViewRechargePackages from a dict
view_recharge_packages_from_dict = ViewRechargePackages.from_dict(view_recharge_packages_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


