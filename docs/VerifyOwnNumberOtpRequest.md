# VerifyOwnNumberOtpRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**code** | **str** |  | [optional] 

## Example

```python
from clicksend.models.verify_own_number_otp_request import VerifyOwnNumberOtpRequest

# TODO update the JSON string below
json = "{}"
# create an instance of VerifyOwnNumberOtpRequest from a JSON string
verify_own_number_otp_request_instance = VerifyOwnNumberOtpRequest.from_json(json)
# print the JSON string representation of the object
print(VerifyOwnNumberOtpRequest.to_json())

# convert the object into a dict
verify_own_number_otp_request_dict = verify_own_number_otp_request_instance.to_dict()
# create an instance of VerifyOwnNumberOtpRequest from a dict
verify_own_number_otp_request_from_dict = VerifyOwnNumberOtpRequest.from_dict(verify_own_number_otp_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


