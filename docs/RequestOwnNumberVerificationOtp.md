# RequestOwnNumberVerificationOtp


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
from clicksend.models.request_own_number_verification_otp import RequestOwnNumberVerificationOtp

# TODO update the JSON string below
json = "{}"
# create an instance of RequestOwnNumberVerificationOtp from a JSON string
request_own_number_verification_otp_instance = RequestOwnNumberVerificationOtp.from_json(json)
# print the JSON string representation of the object
print(RequestOwnNumberVerificationOtp.to_json())

# convert the object into a dict
request_own_number_verification_otp_dict = request_own_number_verification_otp_instance.to_dict()
# create an instance of RequestOwnNumberVerificationOtp from a dict
request_own_number_verification_otp_from_dict = RequestOwnNumberVerificationOtp.from_dict(request_own_number_verification_otp_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


