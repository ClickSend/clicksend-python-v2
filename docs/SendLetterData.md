# SendLetterData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipients** | [**List[Recipient]**](Recipient.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from clicksend.models.send_letter_data import SendLetterData

# TODO update the JSON string below
json = "{}"
# create an instance of SendLetterData from a JSON string
send_letter_data_instance = SendLetterData.from_json(json)
# print the JSON string representation of the object
print(SendLetterData.to_json())

# convert the object into a dict
send_letter_data_dict = send_letter_data_instance.to_dict()
# create an instance of SendLetterData from a dict
send_letter_data_from_dict = SendLetterData.from_dict(send_letter_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


