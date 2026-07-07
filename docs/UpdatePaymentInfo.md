# UpdatePaymentInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**UpdatePaymentInfoData**](UpdatePaymentInfoData.md) |  | [optional] 

## Example

```python
from clicksend.models.update_payment_info import UpdatePaymentInfo

# TODO update the JSON string below
json = "{}"
# create an instance of UpdatePaymentInfo from a JSON string
update_payment_info_instance = UpdatePaymentInfo.from_json(json)
# print the JSON string representation of the object
print(UpdatePaymentInfo.to_json())

# convert the object into a dict
update_payment_info_dict = update_payment_info_instance.to_dict()
# create an instance of UpdatePaymentInfo from a dict
update_payment_info_from_dict = UpdatePaymentInfo.from_dict(update_payment_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


