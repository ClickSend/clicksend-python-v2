# UpdateSubaccountRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_sms** | **int** |  | [optional] 
**email** | **str** |  | [optional] 

## Example

```python
from clicksend.models.update_subaccount_request import UpdateSubaccountRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSubaccountRequest from a JSON string
update_subaccount_request_instance = UpdateSubaccountRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateSubaccountRequest.to_json())

# convert the object into a dict
update_subaccount_request_dict = update_subaccount_request_instance.to_dict()
# create an instance of UpdateSubaccountRequest from a dict
update_subaccount_request_from_dict = UpdateSubaccountRequest.from_dict(update_subaccount_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


