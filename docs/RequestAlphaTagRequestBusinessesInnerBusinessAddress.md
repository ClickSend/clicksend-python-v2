# RequestAlphaTagRequestBusinessesInnerBusinessAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**addr_line1** | **str** |  | 
**addr_line2** | **str** |  | [optional] 
**city** | **str** |  | 
**state** | **str** |  | 
**postal** | **str** |  | 

## Example

```python
from clicksend.models.request_alpha_tag_request_businesses_inner_business_address import RequestAlphaTagRequestBusinessesInnerBusinessAddress

# TODO update the JSON string below
json = "{}"
# create an instance of RequestAlphaTagRequestBusinessesInnerBusinessAddress from a JSON string
request_alpha_tag_request_businesses_inner_business_address_instance = RequestAlphaTagRequestBusinessesInnerBusinessAddress.from_json(json)
# print the JSON string representation of the object
print(RequestAlphaTagRequestBusinessesInnerBusinessAddress.to_json())

# convert the object into a dict
request_alpha_tag_request_businesses_inner_business_address_dict = request_alpha_tag_request_businesses_inner_business_address_instance.to_dict()
# create an instance of RequestAlphaTagRequestBusinessesInnerBusinessAddress from a dict
request_alpha_tag_request_businesses_inner_business_address_from_dict = RequestAlphaTagRequestBusinessesInnerBusinessAddress.from_dict(request_alpha_tag_request_businesses_inner_business_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


