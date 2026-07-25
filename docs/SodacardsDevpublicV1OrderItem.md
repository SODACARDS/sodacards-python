# SodacardsDevpublicV1OrderItem

OrderItem is one line of an order.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product_id** | **str** | product_id is the product ordered on this line. | [optional] 
**name** | **str** | name is the product name at order time. | [optional] 
**unit_price** | [**SodacardsDevpublicV1Money**](SodacardsDevpublicV1Money.md) | unit_price is the price of one unit, in FCFA. | [optional] 
**quantity** | **int** | quantity is how many units were ordered. | [optional] 
**line_total** | [**SodacardsDevpublicV1Money**](SodacardsDevpublicV1Money.md) | line_total is unit_price times quantity, in FCFA. | [optional] 
**input_fields** | **Dict[str, str]** | input_fields are the purchase-form values submitted for this line. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_order_item import SodacardsDevpublicV1OrderItem

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1OrderItem from a JSON string
sodacards_devpublic_v1_order_item_instance = SodacardsDevpublicV1OrderItem.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1OrderItem.to_json())

# convert the object into a dict
sodacards_devpublic_v1_order_item_dict = sodacards_devpublic_v1_order_item_instance.to_dict()
# create an instance of SodacardsDevpublicV1OrderItem from a dict
sodacards_devpublic_v1_order_item_from_dict = SodacardsDevpublicV1OrderItem.from_dict(sodacards_devpublic_v1_order_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


