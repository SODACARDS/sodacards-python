# SodacardsDevpublicV1DeleteWebhookRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id is the webhook endpoint to remove. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_delete_webhook_request import SodacardsDevpublicV1DeleteWebhookRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1DeleteWebhookRequest from a JSON string
sodacards_devpublic_v1_delete_webhook_request_instance = SodacardsDevpublicV1DeleteWebhookRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1DeleteWebhookRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_delete_webhook_request_dict = sodacards_devpublic_v1_delete_webhook_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1DeleteWebhookRequest from a dict
sodacards_devpublic_v1_delete_webhook_request_from_dict = SodacardsDevpublicV1DeleteWebhookRequest.from_dict(sodacards_devpublic_v1_delete_webhook_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


