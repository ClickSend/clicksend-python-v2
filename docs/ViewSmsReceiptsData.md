# ViewSmsReceiptsData

The parameters related to the total message receipts shown. The response will depend on the pagination parameters, specified in the query parameters.

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
**data** | [**List[SmsReceipt]**](SmsReceipt.md) | The parameters related to the actual message receipts. | [optional] 

## Example

```python
from clicksend.models.view_sms_receipts_data import ViewSmsReceiptsData

# TODO update the JSON string below
json = "{}"
# create an instance of ViewSmsReceiptsData from a JSON string
view_sms_receipts_data_instance = ViewSmsReceiptsData.from_json(json)
# print the JSON string representation of the object
print(ViewSmsReceiptsData.to_json())

# convert the object into a dict
view_sms_receipts_data_dict = view_sms_receipts_data_instance.to_dict()
# create an instance of ViewSmsReceiptsData from a dict
view_sms_receipts_data_from_dict = ViewSmsReceiptsData.from_dict(view_sms_receipts_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


