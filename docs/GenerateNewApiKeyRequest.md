# GenerateNewApiKeyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_sms** | **int** |  | [optional] 
**email** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 

## Example

```python
from clicksend.models.generate_new_api_key_request import GenerateNewApiKeyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GenerateNewApiKeyRequest from a JSON string
generate_new_api_key_request_instance = GenerateNewApiKeyRequest.from_json(json)
# print the JSON string representation of the object
print(GenerateNewApiKeyRequest.to_json())

# convert the object into a dict
generate_new_api_key_request_dict = generate_new_api_key_request_instance.to_dict()
# create an instance of GenerateNewApiKeyRequest from a dict
generate_new_api_key_request_from_dict = GenerateNewApiKeyRequest.from_dict(generate_new_api_key_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


