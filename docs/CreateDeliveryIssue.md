# CreateDeliveryIssue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **int** | The HTTP status code of the response. | [optional] 
**response_code** | **str** | The response code indicating the status of the operation. | [optional] 
**response_msg** | **str** | A message describing the outcome of the operation. | [optional] 
**data** | [**CreateDeliveryIssueData**](CreateDeliveryIssueData.md) |  | [optional] 

## Example

```python
from clicksend.models.create_delivery_issue import CreateDeliveryIssue

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDeliveryIssue from a JSON string
create_delivery_issue_instance = CreateDeliveryIssue.from_json(json)
# print the JSON string representation of the object
print(CreateDeliveryIssue.to_json())

# convert the object into a dict
create_delivery_issue_dict = create_delivery_issue_instance.to_dict()
# create an instance of CreateDeliveryIssue from a dict
create_delivery_issue_from_dict = CreateDeliveryIssue.from_dict(create_delivery_issue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


