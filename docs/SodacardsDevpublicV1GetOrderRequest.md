# SodacardsDevpublicV1GetOrderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id is the order id, from PlaceOrder. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_get_order_request import SodacardsDevpublicV1GetOrderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1GetOrderRequest from a JSON string
sodacards_devpublic_v1_get_order_request_instance = SodacardsDevpublicV1GetOrderRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1GetOrderRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_get_order_request_dict = sodacards_devpublic_v1_get_order_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1GetOrderRequest from a dict
sodacards_devpublic_v1_get_order_request_from_dict = SodacardsDevpublicV1GetOrderRequest.from_dict(sodacards_devpublic_v1_get_order_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


