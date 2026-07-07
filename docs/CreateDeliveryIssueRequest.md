# CreateDeliveryIssueRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**email_address** | **str** |  | [optional] 
**client_comments** | **str** |  | [optional] 
**support_comments** | **str** |  | [optional] 
**resolved** | **bool** |  | [optional] 

## Example

```python
from clicksend.models.create_delivery_issue_request import CreateDeliveryIssueRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDeliveryIssueRequest from a JSON string
create_delivery_issue_request_instance = CreateDeliveryIssueRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDeliveryIssueRequest.to_json())

# convert the object into a dict
create_delivery_issue_request_dict = create_delivery_issue_request_instance.to_dict()
# create an instance of CreateDeliveryIssueRequest from a dict
create_delivery_issue_request_from_dict = CreateDeliveryIssueRequest.from_dict(create_delivery_issue_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


