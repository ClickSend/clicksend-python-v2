# RequestAlphaTagRequestBusinessesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country** | **str** |  | 
**business_name** | **str** |  | 
**business_relationship** | **str** | Indicates your relationship to the business being registered.  - **PRIMARY**: Your primary business (linked to your ClickSend account). - **ENTITY_ASSOCIATE**: Sending on behalf of another business you represent or own.  | 
**business_info** | [**RequestAlphaTagRequestBusinessesInnerBusinessInfo**](RequestAlphaTagRequestBusinessesInnerBusinessInfo.md) |  | 
**business_address** | [**RequestAlphaTagRequestBusinessesInnerBusinessAddress**](RequestAlphaTagRequestBusinessesInnerBusinessAddress.md) |  | 
**representative** | [**RequestAlphaTagRequestBusinessesInnerRepresentative**](RequestAlphaTagRequestBusinessesInnerRepresentative.md) |  | 
**abn** | **str** | Australian Business Number (ABN), 11 digits | 
**partner_business_name** | **str** | Partner&#39;s business name. **Required** when &#x60;business_relationship&#x60; is &#x60;ENTITY_ASSOCIATE&#x60;. **Forbidden** otherwise.  | [optional] 
**partner_abn** | **str** | Partner&#39;s Australian Business Number (ABN). Must contain only digits. **Required** when &#x60;business_relationship&#x60; is &#x60;ENTITY_ASSOCIATE&#x60;. **Forbidden** otherwise.  | [optional] 
**partner_business_info** | [**RequestAlphaTagRequestBusinessesInnerBusinessInfo**](RequestAlphaTagRequestBusinessesInnerBusinessInfo.md) |  | [optional] 
**partner_business_address** | [**RequestAlphaTagRequestBusinessesInnerBusinessAddress**](RequestAlphaTagRequestBusinessesInnerBusinessAddress.md) |  | [optional] 
**partner_representative** | [**RequestAlphaTagRequestBusinessesInnerPartnerRepresentative**](RequestAlphaTagRequestBusinessesInnerPartnerRepresentative.md) |  | [optional] 

## Example

```python
from clicksend.models.request_alpha_tag_request_businesses_inner import RequestAlphaTagRequestBusinessesInner

# TODO update the JSON string below
json = "{}"
# create an instance of RequestAlphaTagRequestBusinessesInner from a JSON string
request_alpha_tag_request_businesses_inner_instance = RequestAlphaTagRequestBusinessesInner.from_json(json)
# print the JSON string representation of the object
print(RequestAlphaTagRequestBusinessesInner.to_json())

# convert the object into a dict
request_alpha_tag_request_businesses_inner_dict = request_alpha_tag_request_businesses_inner_instance.to_dict()
# create an instance of RequestAlphaTagRequestBusinessesInner from a dict
request_alpha_tag_request_businesses_inner_from_dict = RequestAlphaTagRequestBusinessesInner.from_dict(request_alpha_tag_request_businesses_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


