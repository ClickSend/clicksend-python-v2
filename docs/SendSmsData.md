# SendSmsData

The parameters related to messages.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_price** | **float** | The total price of sending the messages. Visit [this page](/#status-codes) for more information. | [optional] 
**total_count** | **int** | The total number of messages sent from the request. | [optional] 
**queued_count** | **int** | The messages will be put in a queue if it goes through the validation process. The validation process checks whether the **Sender ID** is registered or not. Some countries don&#39;t require messages to go through the validation process.  Messages scheduled to be sent right away will be sent immediately. If not, it will be queued. | [optional] 
**messages** | [**List[SmsSendSms]**](SmsSendSms.md) | The parameters related to messages. | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 
**blocked_count** | **int** | The number of messages unable to be sent. This is often caused by:  - Receipient’s country not enabled for &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/qdavyt16qs-global-sending\&quot;&gt;global sending&lt;/a&gt;.      - **Sender ID** resitriction.      - Number registration restrcition. | [optional] 

## Example

```python
from clicksend.models.send_sms_data import SendSmsData

# TODO update the JSON string below
json = "{}"
# create an instance of SendSmsData from a JSON string
send_sms_data_instance = SendSmsData.from_json(json)
# print the JSON string representation of the object
print(SendSmsData.to_json())

# convert the object into a dict
send_sms_data_dict = send_sms_data_instance.to_dict()
# create an instance of SendSmsData from a dict
send_sms_data_from_dict = SendSmsData.from_dict(send_sms_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


