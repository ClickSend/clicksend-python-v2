# PurchaseDedicatedNumber


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**PurchaseDedicatedNumberData**](PurchaseDedicatedNumberData.md) |  | [optional] 

## Example

```python
from clicksend.models.purchase_dedicated_number import PurchaseDedicatedNumber

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseDedicatedNumber from a JSON string
purchase_dedicated_number_instance = PurchaseDedicatedNumber.from_json(json)
# print the JSON string representation of the object
print(PurchaseDedicatedNumber.to_json())

# convert the object into a dict
purchase_dedicated_number_dict = purchase_dedicated_number_instance.to_dict()
# create an instance of PurchaseDedicatedNumber from a dict
purchase_dedicated_number_from_dict = PurchaseDedicatedNumber.from_dict(purchase_dedicated_number_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


