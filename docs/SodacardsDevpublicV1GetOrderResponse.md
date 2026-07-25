# SodacardsDevpublicV1GetOrderResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order** | [**SodacardsDevpublicV1Order**](SodacardsDevpublicV1Order.md) | order is the requested order. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_get_order_response import SodacardsDevpublicV1GetOrderResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1GetOrderResponse from a JSON string
sodacards_devpublic_v1_get_order_response_instance = SodacardsDevpublicV1GetOrderResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1GetOrderResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_get_order_response_dict = sodacards_devpublic_v1_get_order_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1GetOrderResponse from a dict
sodacards_devpublic_v1_get_order_response_from_dict = SodacardsDevpublicV1GetOrderResponse.from_dict(sodacards_devpublic_v1_get_order_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


