# ViewSmsInboundAutomationsData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** | The total number of items available for viewing. | [optional] 
**per_page** | **int** | The number of items returned per page. This is specified in the limit parameter. You can have 100 items at maximum, and 15 at minimum. | [optional] 
**current_page** | **int** | The current page number. | [optional] 
**last_page** | **int** | The last page number. | [optional] 
**next_page_url** | **str** | A URL of the next page. It will return **null** if there’s no next page. | [optional] 
**prev_page_url** | **str** | A URL of the previous page. It will return **null** if there’s no previous page. | [optional] 
**var_from** | **int** | The number of the first result in the current page. | [optional] 
**to** | **int** | The number of the last result in the current page. | [optional] 
**first_page_url** | **str** | The URL of the first page of records. | [optional] 
**last_page_url** | **str** | The URL of the last page of records. | [optional] 
**path** | **str** | The base URL path used to build pagination links. | [optional] 
**links** | [**List[ViewListsDataLinksInner]**](ViewListsDataLinksInner.md) | The list of pagination links. | [optional] 
**data** | [**List[SmsInboundRule]**](SmsInboundRule.md) |  | [optional] 

## Example

```python
from clicksend.models.view_sms_inbound_automations_data import ViewSmsInboundAutomationsData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsInboundAutomationsData from a JSON string
view_sms_inbound_automations_data_instance = ViewSmsInboundAutomationsData.from_json(json)
# print the JSON string representation of the object
print(ViewSmsInboundAutomationsData.to_json())

# convert the object into a dict
view_sms_inbound_automations_data_dict = view_sms_inbound_automations_data_instance.to_dict()
# create an instance of ViewSmsInboundAutomationsData from a dict
view_sms_inbound_automations_data_from_dict = ViewSmsInboundAutomationsData.from_dict(view_sms_inbound_automations_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


