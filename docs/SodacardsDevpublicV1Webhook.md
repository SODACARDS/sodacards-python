# SodacardsDevpublicV1Webhook

Webhook is a registered endpoint. It never carries the signing secret.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id identifies the endpoint. | [optional] 
**url** | **str** | url is the HTTPS endpoint events are delivered to. | [optional] 
**events** | **List[str]** | events are the subscribed event types. | [optional] 
**active** | **bool** | active is whether deliveries are currently sent to this endpoint. | [optional] 
**created_at** | **str** | created_at is when the endpoint was registered (RFC 3339). | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_webhook import SodacardsDevpublicV1Webhook

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1Webhook from a JSON string
sodacards_devpublic_v1_webhook_instance = SodacardsDevpublicV1Webhook.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1Webhook.to_json())

# convert the object into a dict
sodacards_devpublic_v1_webhook_dict = sodacards_devpublic_v1_webhook_instance.to_dict()
# create an instance of SodacardsDevpublicV1Webhook from a dict
sodacards_devpublic_v1_webhook_from_dict = SodacardsDevpublicV1Webhook.from_dict(sodacards_devpublic_v1_webhook_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


