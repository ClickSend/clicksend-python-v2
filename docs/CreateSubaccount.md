# CreateSubaccount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**Subaccount**](Subaccount.md) |  | [optional] 

## Example

```python
from clicksend.models.create_subaccount import CreateSubaccount

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSubaccount from a JSON string
create_subaccount_instance = CreateSubaccount.from_json(json)
# print the JSON string representation of the object
print(CreateSubaccount.to_json())

# convert the object into a dict
create_subaccount_dict = create_subaccount_instance.to_dict()
# create an instance of CreateSubaccount from a dict
create_subaccount_from_dict = CreateSubaccount.from_dict(create_subaccount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


