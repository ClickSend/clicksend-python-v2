# SmsCampaignSendersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipient_country_code** | **str** | Recipient ISO country code | [optional] 
**sender_id** | **str** | The sender ID you specified in the request. This parameter would not be returned if you did specify it in the SMS campaign. | [optional] 
**sender_type** | **str** | The type of sender ID you specified in the request. This parameter would not be returned if you did specify it in the SMS campaign. | [optional] 
**sender_country_code** | **str** | The country code of the sender you specified in the request. It is in two-letter format (e.g. US, UK, AU, NZ, &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/7wtbhhy6sy-country-code-calling-code-list\&quot; target&#x3D;\&quot;_blank\&quot;&gt;etc&lt;/a&gt;).  For certain countries, you can receive SMS from abroad. This parameter would not be returned if you did specify it in the SMS campaign. | [optional] 

## Example

```python
from clicksend.models.sms_campaign_senders_inner import SmsCampaignSendersInner

# TODO update the JSON string below
json = "{}"
# create an instance of SmsCampaignSendersInner from a JSON string
sms_campaign_senders_inner_instance = SmsCampaignSendersInner.from_json(json)
# print the JSON string representation of the object
print(SmsCampaignSendersInner.to_json())

# convert the object into a dict
sms_campaign_senders_inner_dict = sms_campaign_senders_inner_instance.to_dict()
# create an instance of SmsCampaignSendersInner from a dict
sms_campaign_senders_inner_from_dict = SmsCampaignSendersInner.from_dict(sms_campaign_senders_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


