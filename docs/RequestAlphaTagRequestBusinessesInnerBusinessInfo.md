# RequestAlphaTagRequestBusinessesInnerBusinessInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**website** | **str** | Business website URL | 
**phone_number** | **str** | E.164 or local format | 

## Example

```python
from clicksend.models.request_alpha_tag_request_businesses_inner_business_info import RequestAlphaTagRequestBusinessesInnerBusinessInfo

# TODO update the JSON string below
json = "{}"
# create an instance of RequestAlphaTagRequestBusinessesInnerBusinessInfo from a JSON string
request_alpha_tag_request_businesses_inner_business_info_instance = RequestAlphaTagRequestBusinessesInnerBusinessInfo.from_json(json)
# print the JSON string representation of the object
print(RequestAlphaTagRequestBusinessesInnerBusinessInfo.to_json())

# convert the object into a dict
request_alpha_tag_request_businesses_inner_business_info_dict = request_alpha_tag_request_businesses_inner_business_info_instance.to_dict()
# create an instance of RequestAlphaTagRequestBusinessesInnerBusinessInfo from a dict
request_alpha_tag_request_businesses_inner_business_info_from_dict = RequestAlphaTagRequestBusinessesInnerBusinessInfo.from_dict(request_alpha_tag_request_businesses_inner_business_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


