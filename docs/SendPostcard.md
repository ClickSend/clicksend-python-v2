# SendPostcard


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SendPostcardData**](SendPostcardData.md) |  | [optional] 

## Example

```python
from clicksend.models.send_postcard import SendPostcard

# TODO update the JSON string below
json = "{}"
# create an instance of SendPostcard from a JSON string
send_postcard_instance = SendPostcard.from_json(json)
# print the JSON string representation of the object
print(SendPostcard.to_json())

# convert the object into a dict
send_postcard_dict = send_postcard_instance.to_dict()
# create an instance of SendPostcard from a dict
send_postcard_from_dict = SendPostcard.from_dict(send_postcard_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


