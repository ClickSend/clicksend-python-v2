# ViewVoiceLanguagesDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | The code of the language. | [optional] 
**country** | **str** | The country of the language. | [optional] 
**gender** | [**ViewVoiceLanguagesDataInnerGender**](ViewVoiceLanguagesDataInnerGender.md) |  | [optional] 

## Example

```python
from clicksend.models.view_voice_languages_data_inner import ViewVoiceLanguagesDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ViewVoiceLanguagesDataInner from a JSON string
view_voice_languages_data_inner_instance = ViewVoiceLanguagesDataInner.from_json(json)
# print the JSON string representation of the object
print(ViewVoiceLanguagesDataInner.to_json())

# convert the object into a dict
view_voice_languages_data_inner_dict = view_voice_languages_data_inner_instance.to_dict()
# create an instance of ViewVoiceLanguagesDataInner from a dict
view_voice_languages_data_inner_from_dict = ViewVoiceLanguagesDataInner.from_dict(view_voice_languages_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


