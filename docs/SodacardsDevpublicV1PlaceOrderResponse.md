# SodacardsDevpublicV1PlaceOrderResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order** | [**SodacardsDevpublicV1PlacedOrder**](SodacardsDevpublicV1PlacedOrder.md) | order is the accepted order. Its status is pending until fulfillment  completes; poll the order to follow it. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_place_order_response import SodacardsDevpublicV1PlaceOrderResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1PlaceOrderResponse from a JSON string
sodacards_devpublic_v1_place_order_response_instance = SodacardsDevpublicV1PlaceOrderResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1PlaceOrderResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_place_order_response_dict = sodacards_devpublic_v1_place_order_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1PlaceOrderResponse from a dict
sodacards_devpublic_v1_place_order_response_from_dict = SodacardsDevpublicV1PlaceOrderResponse.from_dict(sodacards_devpublic_v1_place_order_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


