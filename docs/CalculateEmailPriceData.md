# CalculateEmailPriceData


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

## Example

```python
from clicksend.models.calculate_email_price_data import CalculateEmailPriceData

# TODO update the JSON string below
json = "{}"
# create an instance of CalculateEmailPriceData from a JSON string
calculate_email_price_data_instance = CalculateEmailPriceData.from_json(json)
# print the JSON string representation of the object
print(CalculateEmailPriceData.to_json())

# convert the object into a dict
calculate_email_price_data_dict = calculate_email_price_data_instance.to_dict()
# create an instance of CalculateEmailPriceData from a dict
calculate_email_price_data_from_dict = CalculateEmailPriceData.from_dict(calculate_email_price_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


