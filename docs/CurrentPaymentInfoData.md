# CurrentPaymentInfoData

The data returned by the API call.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_number** | **str** | The credit card number. | [optional] 
**expiry_month** | **int** | The credit card expiry month. | [optional] 
**expiry_year** | **int** | The credit card expiry year. | [optional] 
**name** | **str** | The credit card name. | [optional] 

## Example

```python
from clicksend.models.current_payment_info_data import CurrentPaymentInfoData

# TODO update the JSON string below
json = "{}"
# create an instance of CurrentPaymentInfoData from a JSON string
current_payment_info_data_instance = CurrentPaymentInfoData.from_json(json)
# print the JSON string representation of the object
print(CurrentPaymentInfoData.to_json())

# convert the object into a dict
current_payment_info_data_dict = current_payment_info_data_instance.to_dict()
# create an instance of CurrentPaymentInfoData from a dict
current_payment_info_data_from_dict = CurrentPaymentInfoData.from_dict(current_payment_info_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


