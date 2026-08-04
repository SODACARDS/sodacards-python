# SodacardsDevpublicV1RotateWebhookSecretRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id is the webhook endpoint whose signing secret to rotate. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_rotate_webhook_secret_request import SodacardsDevpublicV1RotateWebhookSecretRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1RotateWebhookSecretRequest from a JSON string
sodacards_devpublic_v1_rotate_webhook_secret_request_instance = SodacardsDevpublicV1RotateWebhookSecretRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1RotateWebhookSecretRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_rotate_webhook_secret_request_dict = sodacards_devpublic_v1_rotate_webhook_secret_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1RotateWebhookSecretRequest from a dict
sodacards_devpublic_v1_rotate_webhook_secret_request_from_dict = SodacardsDevpublicV1RotateWebhookSecretRequest.from_dict(sodacards_devpublic_v1_rotate_webhook_secret_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


