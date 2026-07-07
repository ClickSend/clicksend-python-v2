# RequestAlphaTagRequestBusinessesInnerPartnerRepresentative

Partner's representative details. **Required** when `business_relationship` is `ENTITY_ASSOCIATE`. **Forbidden** otherwise. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | 
**last_name** | **str** |  | 
**email** | **str** |  | 
**title** | **str** |  | 

## Example

```python
from clicksend.models.request_alpha_tag_request_businesses_inner_partner_representative import RequestAlphaTagRequestBusinessesInnerPartnerRepresentative

# TODO update the JSON string below
json = "{}"
# create an instance of RequestAlphaTagRequestBusinessesInnerPartnerRepresentative from a JSON string
request_alpha_tag_request_businesses_inner_partner_representative_instance = RequestAlphaTagRequestBusinessesInnerPartnerRepresentative.from_json(json)
# print the JSON string representation of the object
print(RequestAlphaTagRequestBusinessesInnerPartnerRepresentative.to_json())

# convert the object into a dict
request_alpha_tag_request_businesses_inner_partner_representative_dict = request_alpha_tag_request_businesses_inner_partner_representative_instance.to_dict()
# create an instance of RequestAlphaTagRequestBusinessesInnerPartnerRepresentative from a dict
request_alpha_tag_request_businesses_inner_partner_representative_from_dict = RequestAlphaTagRequestBusinessesInnerPartnerRepresentative.from_dict(request_alpha_tag_request_businesses_inner_partner_representative_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


