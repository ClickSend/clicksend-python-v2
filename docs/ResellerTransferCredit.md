# ResellerTransferCredit


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CreateResellerAccountData**](CreateResellerAccountData.md) |  | [optional] 

## Example

```python
from clicksend.models.reseller_transfer_credit import ResellerTransferCredit

# TODO update the JSON string below
json = "{}"
# create an instance of ResellerTransferCredit from a JSON string
reseller_transfer_credit_instance = ResellerTransferCredit.from_json(json)
# print the JSON string representation of the object
print(ResellerTransferCredit.to_json())

# convert the object into a dict
reseller_transfer_credit_dict = reseller_transfer_credit_instance.to_dict()
# create an instance of ResellerTransferCredit from a dict
reseller_transfer_credit_from_dict = ResellerTransferCredit.from_dict(reseller_transfer_credit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


