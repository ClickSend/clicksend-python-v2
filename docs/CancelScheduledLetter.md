# CancelScheduledLetter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **bool** |  | [optional] 

## Example

```python
from clicksend.models.cancel_scheduled_letter import CancelScheduledLetter

# TODO update the JSON string below
json = "{}"
# create an instance of CancelScheduledLetter from a JSON string
cancel_scheduled_letter_instance = CancelScheduledLetter.from_json(json)
# print the JSON string representation of the object
print(CancelScheduledLetter.to_json())

# convert the object into a dict
cancel_scheduled_letter_dict = cancel_scheduled_letter_instance.to_dict()
# create an instance of CancelScheduledLetter from a dict
cancel_scheduled_letter_from_dict = CancelScheduledLetter.from_dict(cancel_scheduled_letter_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


