# UpdatePaymentInfoRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number** | **str** |  | [optional] 
**expiry_month** | **int** |  | [optional] 
**expiry_year** | **int** |  | [optional] 
**cvc** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**bank_name** | **str** |  | [optional] 

## Example

```python
from clicksend.models.update_payment_info_request import UpdatePaymentInfoRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdatePaymentInfoRequest from a JSON string
update_payment_info_request_instance = UpdatePaymentInfoRequest.from_json(json)
# print the JSON string representation of the object
print(UpdatePaymentInfoRequest.to_json())

# convert the object into a dict
update_payment_info_request_dict = update_payment_info_request_instance.to_dict()
# create an instance of UpdatePaymentInfoRequest from a dict
update_payment_info_request_from_dict = UpdatePaymentInfoRequest.from_dict(update_payment_info_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


