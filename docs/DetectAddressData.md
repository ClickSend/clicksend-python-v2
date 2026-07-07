# DetectAddressData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_name** | **str** | The recipient&#39;s name. | [optional] 
**address_line_1** | **str** | The first line of the recipient&#39;s address. | [optional] 
**address_line_2** | **str** | The second line of the recipient&#39;s address (optional). | [optional] 
**address_city** | **str** | The city of the recipient&#39;s address. | [optional] 
**address_state** | **str** | The state or region of the recipient&#39;s address. | [optional] 
**address_postal_code** | **str** | The postal code or ZIP code of the recipient&#39;s address. | [optional] 
**address_country** | **str** | The country of the recipient&#39;s address. | [optional] 

## Example

```python
from clicksend.models.detect_address_data import DetectAddressData

# TODO update the JSON string below
json = "{}"
# create an instance of DetectAddressData from a JSON string
detect_address_data_instance = DetectAddressData.from_json(json)
# print the JSON string representation of the object
print(DetectAddressData.to_json())

# convert the object into a dict
detect_address_data_dict = detect_address_data_instance.to_dict()
# create an instance of DetectAddressData from a dict
detect_address_data_from_dict = DetectAddressData.from_dict(detect_address_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


