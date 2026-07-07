# DefaultSender


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID of the default sender. | 
**user_id** | **int** | User ID from the version 3 system. | 
**subaccount_id** | **int** | Subaccount ID from version 3. | 
**country_code** | **str** | ISO 3166-1 alpha-2 formatted country code. | 
**product_type** | **str** | Type of product for which the setting is applied. | 
**default_sender_strategies** | [**List[DefaultSenderDefaultSenderStrategiesInner]**](DefaultSenderDefaultSenderStrategiesInner.md) | Default sender strategies. Must contain 1 or more objects. | 
**status** | **str** | Overall status of the default sender. | 
**created_timestamp** | **str** | Timestamp of when the default sender was created. Must be in ISO 8601 format. | 
**updated_timestamp** | **str** | Timestamp of the last update to the default sender. Must be in ISO 8601 format. | 

## Example

```python
from clicksend.models.default_sender import DefaultSender

# TODO update the JSON string below
json = "{}"
# create an instance of DefaultSender from a JSON string
default_sender_instance = DefaultSender.from_json(json)
# print the JSON string representation of the object
print(DefaultSender.to_json())

# convert the object into a dict
default_sender_dict = default_sender_instance.to_dict()
# create an instance of DefaultSender from a dict
default_sender_from_dict = DefaultSender.from_dict(default_sender_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


