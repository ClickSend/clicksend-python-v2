# CalculateVoicePrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | Here are your data. | [optional] 
**data** | [**SendVoiceMessageData**](SendVoiceMessageData.md) |  | [optional] 

## Example

```python
from clicksend.models.calculate_voice_price import CalculateVoicePrice

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateVoicePrice from a JSON string
calculate_voice_price_instance = CalculateVoicePrice.from_json(json)
# print the JSON string representation of the object
print(CalculateVoicePrice.to_json())

# convert the object into a dict
calculate_voice_price_dict = calculate_voice_price_instance.to_dict()
# create an instance of CalculateVoicePrice from a dict
calculate_voice_price_from_dict = CalculateVoicePrice.from_dict(calculate_voice_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


