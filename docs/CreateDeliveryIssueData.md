# CreateDeliveryIssueData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**issue_id** | **int** | The ID of the created delivery issue. | [optional] 
**user_id** | **int** | The ID of the user who created the delivery issue. | [optional] 
**message_id** | **str** | The ID of the message associated with the delivery issue. | [optional] 
**type** | **str** | The type of delivery issue. | [optional] 
**description** | **str** | The description of the delivery issue. | [optional] 
**date_added** | **int** | The timestamp of when the delivery issue was created. | [optional] 
**email_address** | **str** | The email address associated with the delivery issue. | [optional] 

## Example

```python
from clicksend.models.create_delivery_issue_data import CreateDeliveryIssueData

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDeliveryIssueData from a JSON string
create_delivery_issue_data_instance = CreateDeliveryIssueData.from_json(json)
# print the JSON string representation of the object
print(CreateDeliveryIssueData.to_json())

# convert the object into a dict
create_delivery_issue_data_dict = create_delivery_issue_data_instance.to_dict()
# create an instance of CreateDeliveryIssueData from a dict
create_delivery_issue_data_from_dict = CreateDeliveryIssueData.from_dict(create_delivery_issue_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


