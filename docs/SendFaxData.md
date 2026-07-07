# SendFaxData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_price** | **float** | The total price of the fax. | [optional] 
**total_count** | **str** | The total count of the fax. | [optional] 
**queued_count** | **str** | The count of the queued fax. | [optional] 
**messages** | [**List[Fax]**](Fax.md) | The list of messages that were sent. | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.send_fax_data import SendFaxData

# TODO update the JSON string below
json = "{}"
# create an instance of SendFaxData from a JSON string
send_fax_data_instance = SendFaxData.from_json(json)
# print the JSON string representation of the object
print(SendFaxData.to_json())

# convert the object into a dict
send_fax_data_dict = send_fax_data_instance.to_dict()
# create an instance of SendFaxData from a dict
send_fax_data_from_dict = SendFaxData.from_dict(send_fax_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


