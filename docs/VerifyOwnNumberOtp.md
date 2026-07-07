# VerifyOwnNumberOtp


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | The ID of the verification request. | [optional] 
**own_number_id** | **str** | The ID of the own number. | [optional] 
**status** | **str** | The status of the verification request. | [optional] 
**expires_timestamp** | **str** | The expiration timestamp of the verification request. | [optional] 
**remaining_attempts** | **float** | The number of remaining attempts. | [optional] 
**created_timestamp** | **str** | The creation timestamp of the verification request. | [optional] 
**updated_timestamp** | **str** | The last update timestamp of the verification request. | [optional] 

## Example

```python
from clicksend.models.verify_own_number_otp import VerifyOwnNumberOtp

# TODO update the JSON string below
json = "{}"
# create an instance of VerifyOwnNumberOtp from a JSON string
verify_own_number_otp_instance = VerifyOwnNumberOtp.from_json(json)
# print the JSON string representation of the object
print(VerifyOwnNumberOtp.to_json())

# convert the object into a dict
verify_own_number_otp_dict = verify_own_number_otp_instance.to_dict()
# create an instance of VerifyOwnNumberOtp from a dict
verify_own_number_otp_from_dict = VerifyOwnNumberOtp.from_dict(verify_own_number_otp_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


