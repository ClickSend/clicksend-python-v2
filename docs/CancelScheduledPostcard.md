# CancelScheduledPostcard


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | **bool** |  | [optional] 

## Example

```python
from clicksend.models.cancel_scheduled_postcard import CancelScheduledPostcard

# TODO update the JSON string below
json = "{}"
# create an instance of CancelScheduledPostcard from a JSON string
cancel_scheduled_postcard_instance = CancelScheduledPostcard.from_json(json)
# print the JSON string representation of the object
print(CancelScheduledPostcard.to_json())

# convert the object into a dict
cancel_scheduled_postcard_dict = cancel_scheduled_postcard_instance.to_dict()
# create an instance of CancelScheduledPostcard from a dict
cancel_scheduled_postcard_from_dict = CancelScheduledPostcard.from_dict(cancel_scheduled_postcard_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


