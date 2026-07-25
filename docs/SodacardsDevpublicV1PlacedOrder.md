# SodacardsDevpublicV1PlacedOrder

PlacedOrder is the accepted order: its id, the amount charged to the wallet in  FCFA, and its current status.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id identifies the order; use it to poll the order and reveal its codes. | [optional] 
**status** | **str** | status is the order&#39;s current state, e.g. \&quot;pending\&quot;, \&quot;processing\&quot;,  \&quot;completed\&quot;, \&quot;partially_completed\&quot;, \&quot;failed\&quot; or \&quot;refunded\&quot;. | [optional] 
**total** | [**SodacardsDevpublicV1Money**](SodacardsDevpublicV1Money.md) | total is the amount charged to the reseller&#39;s wallet, in FCFA. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_placed_order import SodacardsDevpublicV1PlacedOrder

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1PlacedOrder from a JSON string
sodacards_devpublic_v1_placed_order_instance = SodacardsDevpublicV1PlacedOrder.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1PlacedOrder.to_json())

# convert the object into a dict
sodacards_devpublic_v1_placed_order_dict = sodacards_devpublic_v1_placed_order_instance.to_dict()
# create an instance of SodacardsDevpublicV1PlacedOrder from a dict
sodacards_devpublic_v1_placed_order_from_dict = SodacardsDevpublicV1PlacedOrder.from_dict(sodacards_devpublic_v1_placed_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


