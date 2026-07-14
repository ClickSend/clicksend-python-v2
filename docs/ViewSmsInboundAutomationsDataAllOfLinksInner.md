# ViewSmsInboundAutomationsDataAllOfLinksInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | The URL of this page link. | [optional] 
**label** | **str** | The display label for this page link. | [optional] 
**page** | **int** | The page number this link points to. | [optional] 
**active** | **bool** | Whether this link represents the current page. | [optional] 

## Example

```python
from clicksend.models.view_sms_inbound_automations_data_all_of_links_inner import ViewSmsInboundAutomationsDataAllOfLinksInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsInboundAutomationsDataAllOfLinksInner from a JSON string
view_sms_inbound_automations_data_all_of_links_inner_instance = ViewSmsInboundAutomationsDataAllOfLinksInner.from_json(json)
# print the JSON string representation of the object
print(ViewSmsInboundAutomationsDataAllOfLinksInner.to_json())

# convert the object into a dict
view_sms_inbound_automations_data_all_of_links_inner_dict = view_sms_inbound_automations_data_all_of_links_inner_instance.to_dict()
# create an instance of ViewSmsInboundAutomationsDataAllOfLinksInner from a dict
view_sms_inbound_automations_data_all_of_links_inner_from_dict = ViewSmsInboundAutomationsDataAllOfLinksInner.from_dict(view_sms_inbound_automations_data_all_of_links_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


