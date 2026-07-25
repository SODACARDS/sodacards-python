# SodacardsDevpublicV1RegisterWebhookRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | url is the HTTPS endpoint to deliver events to. | [optional] 
**events** | **List[str]** | events are the event types to subscribe to (at least one), e.g.  \&quot;order.fulfilled\&quot;, \&quot;order.needs_attention\&quot;, \&quot;order.refunded\&quot;, \&quot;wallet.low_balance\&quot;,  \&quot;wallet.credited\&quot;. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_register_webhook_request import SodacardsDevpublicV1RegisterWebhookRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1RegisterWebhookRequest from a JSON string
sodacards_devpublic_v1_register_webhook_request_instance = SodacardsDevpublicV1RegisterWebhookRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1RegisterWebhookRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_register_webhook_request_dict = sodacards_devpublic_v1_register_webhook_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1RegisterWebhookRequest from a dict
sodacards_devpublic_v1_register_webhook_request_from_dict = SodacardsDevpublicV1RegisterWebhookRequest.from_dict(sodacards_devpublic_v1_register_webhook_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


