# SendPostcardData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_price** | **float** | The total price of the postcard. | [optional] 
**total_count** | **int** | The total count of the postcard. | [optional] 
**queued_count** | **int** | The count of the queued postcard. | [optional] 
**recipients** | [**List[PostcardRecipient]**](PostcardRecipient.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.send_postcard_data import SendPostcardData

# TODO update the JSON string below
json = "{}"
# create an instance of SendPostcardData from a JSON string
send_postcard_data_instance = SendPostcardData.from_json(json)
# print the JSON string representation of the object
print(SendPostcardData.to_json())

# convert the object into a dict
send_postcard_data_dict = send_postcard_data_instance.to_dict()
# create an instance of SendPostcardData from a dict
send_postcard_data_from_dict = SendPostcardData.from_dict(send_postcard_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


