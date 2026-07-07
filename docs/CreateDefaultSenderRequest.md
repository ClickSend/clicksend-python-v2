# CreateDefaultSenderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country_code** | **str** | The country code of the recipient. Must be a valid ISO 3166-1 alpha-2 country code. | 
**product_type** | **str** | The type of product for the assignment. Support for additional types coming soon. | 
**default_sender_strategies** | [**List[CreateDefaultSenderRequestDefaultSenderStrategiesInner]**](CreateDefaultSenderRequestDefaultSenderStrategiesInner.md) | Array detailing sender strategies. Must contain exactly 1 element. Multiple strategies support coming soon. | 

## Example

```python
from clicksend.models.create_default_sender_request import CreateDefaultSenderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDefaultSenderRequest from a JSON string
create_default_sender_request_instance = CreateDefaultSenderRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDefaultSenderRequest.to_json())

# convert the object into a dict
create_default_sender_request_dict = create_default_sender_request_instance.to_dict()
# create an instance of CreateDefaultSenderRequest from a dict
create_default_sender_request_from_dict = CreateDefaultSenderRequest.from_dict(create_default_sender_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


