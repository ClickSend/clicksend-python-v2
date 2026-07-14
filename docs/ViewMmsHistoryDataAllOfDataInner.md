# ViewMmsHistoryDataAllOfDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**direction** | **str** | The direction of the message (in or out). | [optional] 
**var_date** | **str** | The date of the message. | [optional] 
**to** | **str** | The recipient of the message. | [optional] 
**body** | **str** | The body of the message. | [optional] 
**subject** | **str** | The subject of the message. | [optional] 
**priority** | **int** | The priority of the message. | [optional] 
**media_file_url** | **str** | A temporary, signed URL to download the message&#39;s media attachment. | [optional] 
**status** | **str** | The status of the message. | [optional] 
**var_from** | **str** | The sender of the message. | [optional] 
**schedule** | **str** | The schedule time of the message. | [optional] 
**date_added** | **int** | The Unix timestamp when the message was added. | [optional] 
**status_code** | **str** | The status code (if applicable). | [optional] 
**status_text** | **str** | The status text (if applicable). | [optional] 
**error_code** | **str** | The error code (if applicable). | [optional] 
**error_text** | **str** | The error text (if applicable). | [optional] 
**message_id** | **str** | The ID of the message. | [optional] 
**message_parts** | **str** | The number of parts the message was split into. | [optional] 
**message_price** | **str** | The price of the message. | [optional] 
**from_email** | **str** | The email of the sender (if applicable). | [optional] 
**list_id** | **str** | The ID of the list (if applicable). | [optional] 
**custom_string** | **str** | Custom string associated with the message. | [optional] 
**contact_id** | **int** | The ID of the contact. | [optional] 
**user_id** | **int** | The ID of the user. | [optional] 
**subaccount_id** | **int** | The ID of the subaccount. | [optional] 
**country** | **str** | The country code. | [optional] 
**carrier** | **str** | The carrier information. | [optional] 
**first_name** | **str** | The first name of the sender. | [optional] 
**last_name** | **str** | The last name of the sender. | [optional] 
**api_username** | **str** | The API username associated with the message. | [optional] 

## Example

```python
from clicksend.models.view_mms_history_data_all_of_data_inner import ViewMmsHistoryDataAllOfDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewMmsHistoryDataAllOfDataInner from a JSON string
view_mms_history_data_all_of_data_inner_instance = ViewMmsHistoryDataAllOfDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewMmsHistoryDataAllOfDataInner.to_json())

# convert the object into a dict
view_mms_history_data_all_of_data_inner_dict = view_mms_history_data_all_of_data_inner_instance.to_dict()
# create an instance of ViewMmsHistoryDataAllOfDataInner from a dict
view_mms_history_data_all_of_data_inner_from_dict = ViewMmsHistoryDataAllOfDataInner.from_dict(view_mms_history_data_all_of_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


