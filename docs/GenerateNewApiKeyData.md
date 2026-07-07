# GenerateNewApiKeyData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_key** | **str** | The new API key | [optional] 

## Example

```python
from clicksend.models.generate_new_api_key_data import GenerateNewApiKeyData

# TODO update the JSON string below
json = "{}"
# create an instance of GenerateNewApiKeyData from a JSON string
generate_new_api_key_data_instance = GenerateNewApiKeyData.from_json(json)
# print the JSON string representation of the object
print(GenerateNewApiKeyData.to_json())

# convert the object into a dict
generate_new_api_key_data_dict = generate_new_api_key_data_instance.to_dict()
# create an instance of GenerateNewApiKeyData from a dict
generate_new_api_key_data_from_dict = GenerateNewApiKeyData.from_dict(generate_new_api_key_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


