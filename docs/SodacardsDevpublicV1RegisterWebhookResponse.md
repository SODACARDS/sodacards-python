# SodacardsDevpublicV1RegisterWebhookResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**webhook** | [**SodacardsDevpublicV1Webhook**](SodacardsDevpublicV1Webhook.md) | webhook is the registered endpoint. | [optional] 
**secret** | **str** | secret is the signing secret, shown only once. Store it; verify each delivery  with it. It is never returned again. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_register_webhook_response import SodacardsDevpublicV1RegisterWebhookResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1RegisterWebhookResponse from a JSON string
sodacards_devpublic_v1_register_webhook_response_instance = SodacardsDevpublicV1RegisterWebhookResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1RegisterWebhookResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_register_webhook_response_dict = sodacards_devpublic_v1_register_webhook_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1RegisterWebhookResponse from a dict
sodacards_devpublic_v1_register_webhook_response_from_dict = SodacardsDevpublicV1RegisterWebhookResponse.from_dict(sodacards_devpublic_v1_register_webhook_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


