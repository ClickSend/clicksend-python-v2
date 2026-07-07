# SendFax


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**SendFaxData**](SendFaxData.md) |  | [optional] 

## Example

```python
from clicksend.models.send_fax import SendFax

# TODO update the JSON string below
json = "{}"
# create an instance of SendFax from a JSON string
send_fax_instance = SendFax.from_json(json)
# print the JSON string representation of the object
print(SendFax.to_json())

# convert the object into a dict
send_fax_dict = send_fax_instance.to_dict()
# create an instance of SendFax from a dict
send_fax_from_dict = SendFax.from_dict(send_fax_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


