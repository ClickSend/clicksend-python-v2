# UpdatePaymentInfoData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **str** | The token. | [optional] 

## Example

```python
from clicksend.models.update_payment_info_data import UpdatePaymentInfoData

# TODO update the JSON string below
json = "{}"
# create an instance of UpdatePaymentInfoData from a JSON string
update_payment_info_data_instance = UpdatePaymentInfoData.from_json(json)
# print the JSON string representation of the object
print(UpdatePaymentInfoData.to_json())

# convert the object into a dict
update_payment_info_data_dict = update_payment_info_data_instance.to_dict()
# create an instance of UpdatePaymentInfoData from a dict
update_payment_info_data_from_dict = UpdatePaymentInfoData.from_dict(update_payment_info_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


