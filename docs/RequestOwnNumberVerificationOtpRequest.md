# RequestOwnNumberVerificationOtpRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**country** | **str** |  | [optional] 

## Example

```python
from clicksend.models.request_own_number_verification_otp_request import RequestOwnNumberVerificationOtpRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RequestOwnNumberVerificationOtpRequest from a JSON string
request_own_number_verification_otp_request_instance = RequestOwnNumberVerificationOtpRequest.from_json(json)
# print the JSON string representation of the object
print(RequestOwnNumberVerificationOtpRequest.to_json())

# convert the object into a dict
request_own_number_verification_otp_request_dict = request_own_number_verification_otp_request_instance.to_dict()
# create an instance of RequestOwnNumberVerificationOtpRequest from a dict
request_own_number_verification_otp_request_from_dict = RequestOwnNumberVerificationOtpRequest.from_dict(request_own_number_verification_otp_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


