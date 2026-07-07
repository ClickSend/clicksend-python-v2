# SendMmsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_price** | **float** | The total price of the MMS messages. | [optional] 
**total_count** | **int** | The total count of the MMS messages. | [optional] 
**queued_count** | **int** | The count of the queued MMS messages. | [optional] 
**messages** | [**List[Mms]**](Mms.md) |  | [optional] 

## Example

```python
from clicksend.models.send_mms_data import SendMmsData

# TODO update the JSON string below
json = "{}"
# create an instance of SendMmsData from a JSON string
send_mms_data_instance = SendMmsData.from_json(json)
# print the JSON string representation of the object
print(SendMmsData.to_json())

# convert the object into a dict
send_mms_data_dict = send_mms_data_instance.to_dict()
# create an instance of SendMmsData from a dict
send_mms_data_from_dict = SendMmsData.from_dict(send_mms_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


