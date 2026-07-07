# ViewEmailTemplatesData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** | The total number of records in the response. | [optional] 
**per_page** | **int** | The number of records per page. | [optional] 
**current_page** | **int** | The current page number. | [optional] 
**last_page** | **int** | The last page number. | [optional] 
**next_page_url** | **str** | The URL of the next page of records. | [optional] 
**prev_page_url** | **str** | The URL of the previous page of records. | [optional] 
**var_from** | **int** | The index of the first record in the page. | [optional] 
**to** | **int** | The index of the last record in the page. | [optional] 
**data** | [**List[ViewEmailTemplatesDataDataInner]**](ViewEmailTemplatesDataDataInner.md) |  | [optional] 

## Example

```python
from clicksend.models.view_email_templates_data import ViewEmailTemplatesData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewEmailTemplatesData from a JSON string
view_email_templates_data_instance = ViewEmailTemplatesData.from_json(json)
# print the JSON string representation of the object
print(ViewEmailTemplatesData.to_json())

# convert the object into a dict
view_email_templates_data_dict = view_email_templates_data_instance.to_dict()
# create an instance of ViewEmailTemplatesData from a dict
view_email_templates_data_from_dict = ViewEmailTemplatesData.from_dict(view_email_templates_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


