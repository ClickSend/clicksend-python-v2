# CurrentPaymentInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CurrentPaymentInfoData**](CurrentPaymentInfoData.md) |  | [optional] 

## Example

```python
from clicksend.models.current_payment_info import CurrentPaymentInfo

# TODO update the JSON string below
json = "{}"
# create an instance of CurrentPaymentInfo from a JSON string
current_payment_info_instance = CurrentPaymentInfo.from_json(json)
# print the JSON string representation of the object
print(CurrentPaymentInfo.to_json())

# convert the object into a dict
current_payment_info_dict = current_payment_info_instance.to_dict()
# create an instance of CurrentPaymentInfo from a dict
current_payment_info_from_dict = CurrentPaymentInfo.from_dict(current_payment_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


