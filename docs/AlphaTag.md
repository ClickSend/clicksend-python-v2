# AlphaTag


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | The unique identifier for the record. | [optional] 
**account_id** | **str** | The unique identifier for the account. | [optional] 
**workspace_id** | **str** | The unique identifier for the workspace. | [optional] 
**user_id** | **str** | The unique identifier for the user. | [optional] 
**alpha_tag** | **str** | The alpha tag. | [optional] 
**status** | **str** | The status of the record. | [optional] 
**reason** | **str** | The reason for the status. | [optional] 
**countries** | **List[str]** | List of country codes where the alpha tag is requested. If not provided, it means a global alpha tag. | [optional] 
**created_timestamp** | **datetime** | The timestamp when the record was created. | [optional] 
**updated_timestamp** | **datetime** | The timestamp when the record was last updated. | [optional] 

## Example

```python
from clicksend.models.alpha_tag import AlphaTag

# TODO update the JSON string below
json = "{}"
# create an instance of AlphaTag from a JSON string
alpha_tag_instance = AlphaTag.from_json(json)
# print the JSON string representation of the object
print(AlphaTag.to_json())

# convert the object into a dict
alpha_tag_dict = alpha_tag_instance.to_dict()
# create an instance of AlphaTag from a dict
alpha_tag_from_dict = AlphaTag.from_dict(alpha_tag_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


