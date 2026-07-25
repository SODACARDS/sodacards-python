# SodacardsDevpublicV1PlaceOrderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**lines** | [**List[SodacardsDevpublicV1OrderLine]**](SodacardsDevpublicV1OrderLine.md) | lines are the products to buy and how many of each. At least one is required. | [optional] 
**reference** | **str** | reference is an optional identifier you attach to the order to correlate it  with your own system and look it up later. Reusing an Idempotency-Key with a  different reference is a conflict. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_place_order_request import SodacardsDevpublicV1PlaceOrderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1PlaceOrderRequest from a JSON string
sodacards_devpublic_v1_place_order_request_instance = SodacardsDevpublicV1PlaceOrderRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1PlaceOrderRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_place_order_request_dict = sodacards_devpublic_v1_place_order_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1PlaceOrderRequest from a dict
sodacards_devpublic_v1_place_order_request_from_dict = SodacardsDevpublicV1PlaceOrderRequest.from_dict(sodacards_devpublic_v1_place_order_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


