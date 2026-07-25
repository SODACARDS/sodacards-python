# SodacardsDevpublicV1ListWebhooksResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**webhooks** | [**List[SodacardsDevpublicV1Webhook]**](SodacardsDevpublicV1Webhook.md) | webhooks are the reseller&#39;s registered endpoints. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_list_webhooks_response import SodacardsDevpublicV1ListWebhooksResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1ListWebhooksResponse from a JSON string
sodacards_devpublic_v1_list_webhooks_response_instance = SodacardsDevpublicV1ListWebhooksResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1ListWebhooksResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_list_webhooks_response_dict = sodacards_devpublic_v1_list_webhooks_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1ListWebhooksResponse from a dict
sodacards_devpublic_v1_list_webhooks_response_from_dict = SodacardsDevpublicV1ListWebhooksResponse.from_dict(sodacards_devpublic_v1_list_webhooks_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


