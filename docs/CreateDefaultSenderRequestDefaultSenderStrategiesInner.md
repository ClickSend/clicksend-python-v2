# CreateDefaultSenderRequestDefaultSenderStrategiesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sender_type** | **str** | The type of sender for this strategy. | 
**sender_id** | **str** | Unique identifier for the sender. Format varies based on &#x60;sender_type&#x60;: - &#x60;shortcode&#x60;: Numeric, 3-8 digits. - &#x60;longcode&#x60;, &#x60;tollfree&#x60;, &#x60;10DLC&#x60;, &#x60;own_number&#x60;: 2-15 digits, may include &#x60;+&#x60; prefix. - &#x60;alpha_tag&#x60;: 3-11 alphanumeric characters, must include at least one letter or &#x60;+&#x60;. - &#x60;shared_longcode&#x60;: Can be null or empty string.  &gt; **Important:** The &#x60;sender_id&#x60; must be in valid format, owned, and has ready to use status for the corresponding &#x60;sender_type&#x60;.  | 
**sender_country_code** | **str** | The country code of the sender, using the ISO 3166-1 alpha-2 format (e.g., \&quot;US\&quot;).  This field is required in the following cases: - When &#x60;sender_type&#x60; is &#x60;own_number&#x60;, &#x60;longcode&#x60;, &#x60;tollfree&#x60;, or &#x60;10DLC&#x60; - When the &#x60;sender_id&#x60; follows the US/Canada number format (starts with &#x60;+1&#x60;)  For all other cases, this field is optional.  | [optional] 
**note** | **str** | Optional note providing additional context about the sender strategy. | [optional] 

## Example

```python
from clicksend.models.create_default_sender_request_default_sender_strategies_inner import CreateDefaultSenderRequestDefaultSenderStrategiesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDefaultSenderRequestDefaultSenderStrategiesInner from a JSON string
create_default_sender_request_default_sender_strategies_inner_instance = CreateDefaultSenderRequestDefaultSenderStrategiesInner.from_json(json)
# print the JSON string representation of the object
print(CreateDefaultSenderRequestDefaultSenderStrategiesInner.to_json())

# convert the object into a dict
create_default_sender_request_default_sender_strategies_inner_dict = create_default_sender_request_default_sender_strategies_inner_instance.to_dict()
# create an instance of CreateDefaultSenderRequestDefaultSenderStrategiesInner from a dict
create_default_sender_request_default_sender_strategies_inner_from_dict = CreateDefaultSenderRequestDefaultSenderStrategiesInner.from_dict(create_default_sender_request_default_sender_strategies_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


