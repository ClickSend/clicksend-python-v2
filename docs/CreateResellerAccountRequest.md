# CreateResellerAccountRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**user_email** | **str** |  | [optional] 
**user_first_name** | **str** |  | [optional] 
**user_last_name** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**user_phone** | **str** |  | [optional] 
**username** | **str** |  | [optional] 

## Example

```python
from clicksend.models.create_reseller_account_request import CreateResellerAccountRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateResellerAccountRequest from a JSON string
create_reseller_account_request_instance = CreateResellerAccountRequest.from_json(json)
# print the JSON string representation of the object
print(CreateResellerAccountRequest.to_json())

# convert the object into a dict
create_reseller_account_request_dict = create_reseller_account_request_instance.to_dict()
# create an instance of CreateResellerAccountRequest from a dict
create_reseller_account_request_from_dict = CreateResellerAccountRequest.from_dict(create_reseller_account_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


