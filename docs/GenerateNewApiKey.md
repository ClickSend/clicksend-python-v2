# GenerateNewApiKey


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**GenerateNewApiKeyData**](GenerateNewApiKeyData.md) |  | [optional] 

## Example

```python
from clicksend.models.generate_new_api_key import GenerateNewApiKey

# TODO update the JSON string below
json = "{}"
# create an instance of GenerateNewApiKey from a JSON string
generate_new_api_key_instance = GenerateNewApiKey.from_json(json)
# print the JSON string representation of the object
print(GenerateNewApiKey.to_json())

# convert the object into a dict
generate_new_api_key_dict = generate_new_api_key_instance.to_dict()
# create an instance of GenerateNewApiKey from a dict
generate_new_api_key_from_dict = GenerateNewApiKey.from_dict(generate_new_api_key_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


