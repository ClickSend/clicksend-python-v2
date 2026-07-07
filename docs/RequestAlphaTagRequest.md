# RequestAlphaTagRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alpha_tag** | **str** |  | [optional] 
**reason** | **str** |  | [optional] 
**countries** | **List[str]** |  | [optional] 
**businesses** | [**List[RequestAlphaTagRequestBusinessesInner]**](RequestAlphaTagRequestBusinessesInner.md) |  | [optional] 

## Example

```python
from clicksend.models.request_alpha_tag_request import RequestAlphaTagRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RequestAlphaTagRequest from a JSON string
request_alpha_tag_request_instance = RequestAlphaTagRequest.from_json(json)
# print the JSON string representation of the object
print(RequestAlphaTagRequest.to_json())

# convert the object into a dict
request_alpha_tag_request_dict = request_alpha_tag_request_instance.to_dict()
# create an instance of RequestAlphaTagRequest from a dict
request_alpha_tag_request_from_dict = RequestAlphaTagRequest.from_dict(request_alpha_tag_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


