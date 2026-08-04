# SodacardsDevpublicV1RotateWebhookSecretResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**secret** | **str** | secret is the new signing secret, shown only once, like at registration. | [optional] 
**prev_secret_expires_at** | **str** | prev_secret_expires_at is when the previous secret stops being accepted  (RFC 3339). Until then both secrets validate a delivery. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_rotate_webhook_secret_response import SodacardsDevpublicV1RotateWebhookSecretResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1RotateWebhookSecretResponse from a JSON string
sodacards_devpublic_v1_rotate_webhook_secret_response_instance = SodacardsDevpublicV1RotateWebhookSecretResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1RotateWebhookSecretResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_rotate_webhook_secret_response_dict = sodacards_devpublic_v1_rotate_webhook_secret_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1RotateWebhookSecretResponse from a dict
sodacards_devpublic_v1_rotate_webhook_secret_response_from_dict = SodacardsDevpublicV1RotateWebhookSecretResponse.from_dict(sodacards_devpublic_v1_rotate_webhook_secret_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


