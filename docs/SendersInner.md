# SendersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipient_country_code** | **str** | Recipient ISO country code | 
**sender_id** | **str** | The sender ID must be either an alpha tag or a phone number. It is a required field unless the sender type is a &#x60;shared_longcode&#x60;.   If the sender ID is an **alpha tag**, it must be between 3 and 11 characters long and contains only letters, numbers, and pluses.  | [optional] 
**sender_type** | **str** | The type of sender ID, it only supports &#x60;shared_longcode&#x60; at the moment. | [optional] 
**sender_country_code** | **str** | The ISO 3166-1 alpha-2 country code that identifies the country associated with the sender’s number in a shared pool. This is affected only when &#x60;sender_type&#x60; is set to &#x60;shared_longcode&#x60; to determine the appropriate number based on the sender’s geographic location. If this field is not provided or left empty, it will default to the recipient&#39;s country code.  | [optional] 

## Example

```python
from clicksend.models.senders_inner import SendersInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendersInner from a JSON string
senders_inner_instance = SendersInner.from_json(json)
# print the JSON string representation of the object
print(SendersInner.to_json())

# convert the object into a dict
senders_inner_dict = senders_inner_instance.to_dict()
# create an instance of SendersInner from a dict
senders_inner_from_dict = SendersInner.from_dict(senders_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


