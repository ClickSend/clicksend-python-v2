# Attachment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_name** | **str** | The name of the attached file. | [optional] 
**content_type** | **str** | The MIME type of the attached file. | [optional] 
**content_disposition** | **str** | The content disposition of the attached file. | [optional] 
**content_id** | **str** | The content ID of the attached file. | [optional] 
**attachment_file_url** | **str** | The URL to download the attached file. | [optional] 

## Example

```python
from clicksend.models.attachment import Attachment

# TODO update the JSON string below
json = "{}"
# create an instance of Attachment from a JSON string
attachment_instance = Attachment.from_json(json)
# print the JSON string representation of the object
print(Attachment.to_json())

# convert the object into a dict
attachment_dict = attachment_instance.to_dict()
# create an instance of Attachment from a dict
attachment_from_dict = Attachment.from_dict(attachment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


