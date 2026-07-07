# CreateResellerAccount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CreateResellerAccountData**](CreateResellerAccountData.md) |  | [optional] 

## Example

```python
from clicksend.models.create_reseller_account import CreateResellerAccount

# TODO update the JSON string below
json = "{}"
# create an instance of CreateResellerAccount from a JSON string
create_reseller_account_instance = CreateResellerAccount.from_json(json)
# print the JSON string representation of the object
print(CreateResellerAccount.to_json())

# convert the object into a dict
create_reseller_account_dict = create_reseller_account_instance.to_dict()
# create an instance of CreateResellerAccount from a dict
create_reseller_account_from_dict = CreateResellerAccount.from_dict(create_reseller_account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


