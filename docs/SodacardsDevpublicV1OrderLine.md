# SodacardsDevpublicV1OrderLine

OrderLine is one product to buy on an order. input_fields carries the  purchase-form values a product requires (for example a game player id), keyed  by the field name from the product definition.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product_id** | **str** | product_id is the id of the product to buy (a catalog product id). | [optional] 
**quantity** | **int** | quantity is how many units to buy on this line (at least one). | [optional] 
**input_fields** | **Dict[str, str]** | input_fields holds the required purchase-form values, keyed by field name. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_order_line import SodacardsDevpublicV1OrderLine

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1OrderLine from a JSON string
sodacards_devpublic_v1_order_line_instance = SodacardsDevpublicV1OrderLine.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1OrderLine.to_json())

# convert the object into a dict
sodacards_devpublic_v1_order_line_dict = sodacards_devpublic_v1_order_line_instance.to_dict()
# create an instance of SodacardsDevpublicV1OrderLine from a dict
sodacards_devpublic_v1_order_line_from_dict = SodacardsDevpublicV1OrderLine.from_dict(sodacards_devpublic_v1_order_line_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


