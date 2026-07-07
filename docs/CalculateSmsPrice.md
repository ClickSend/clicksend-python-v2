# CalculateSmsPrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **str** | The HTTP code of the response. Visit [this page](/#status-codes) for more information.  This parameter doesn’t reflect the status of each message. Check the status parameter of the message object to view the status of the individual message. | [optional] 
**response_code** | **str** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CalculateSmsPriceData**](CalculateSmsPriceData.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_sms_price import CalculateSmsPrice

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateSmsPrice from a JSON string
calculate_sms_price_instance = CalculateSmsPrice.from_json(json)
# print the JSON string representation of the object
print(CalculateSmsPrice.to_json())

# convert the object into a dict
calculate_sms_price_dict = calculate_sms_price_instance.to_dict()
# create an instance of CalculateSmsPrice from a dict
calculate_sms_price_from_dict = CalculateSmsPrice.from_dict(calculate_sms_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


