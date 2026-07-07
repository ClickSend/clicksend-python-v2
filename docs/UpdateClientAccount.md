# UpdateClientAccount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CreateResellerAccountData**](CreateResellerAccountData.md) |  | [optional] 

## Example

```python
from clicksend.models.update_client_account import UpdateClientAccount

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateClientAccount from a JSON string
update_client_account_instance = UpdateClientAccount.from_json(json)
# print the JSON string representation of the object
print(UpdateClientAccount.to_json())

# convert the object into a dict
update_client_account_dict = update_client_account_instance.to_dict()
# create an instance of UpdateClientAccount from a dict
update_client_account_from_dict = UpdateClientAccount.from_dict(update_client_account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


