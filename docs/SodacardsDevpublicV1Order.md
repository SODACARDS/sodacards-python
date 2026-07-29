# SodacardsDevpublicV1Order

Order is a placed order with its lines and current status. It never carries the  supplier cost.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id identifies the order. | [optional] 
**status** | **str** | status is the order&#39;s current state: \&quot;pending\&quot;, \&quot;processing\&quot;, \&quot;completed\&quot;,  \&quot;failed\&quot; or \&quot;refunded\&quot;. | [optional] 
**total** | [**SodacardsDevpublicV1Money**](SodacardsDevpublicV1Money.md) | total is the amount charged for the order, in the currency of Money. | [optional] 
**created_at** | **str** | created_at is when the order was placed (RFC 3339). | [optional] 
**reference** | **str** | reference is the identifier you attached at creation, empty if none. | [optional] 
**lines** | [**List[SodacardsDevpublicV1OrderItem]**](SodacardsDevpublicV1OrderItem.md) | lines are the ordered products. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_order import SodacardsDevpublicV1Order

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1Order from a JSON string
sodacards_devpublic_v1_order_instance = SodacardsDevpublicV1Order.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1Order.to_json())

# convert the object into a dict
sodacards_devpublic_v1_order_dict = sodacards_devpublic_v1_order_instance.to_dict()
# create an instance of SodacardsDevpublicV1Order from a dict
sodacards_devpublic_v1_order_from_dict = SodacardsDevpublicV1Order.from_dict(sodacards_devpublic_v1_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


