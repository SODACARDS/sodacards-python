# SodacardsDevpublicV1Product

Product is one sellable item in the reseller catalog. Its id is what an order  line references. It never carries the supplier cost or routing.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id identifies the product; use it to place an order for this item. | [optional] 
**name** | **str** | name is the human-readable product name. | [optional] 
**face_value** | [**SodacardsDevpublicV1ProductFaceValue**](SodacardsDevpublicV1ProductFaceValue.md) | face_value is the nominal value printed on the item (e.g. a 10 USD card),  which may differ from the currency the reseller pays in. | [optional] 
**price** | [**SodacardsDevpublicV1Money**](SodacardsDevpublicV1Money.md) | price is what the reseller pays, in the currency of Money. It is absent when the item is not  yet priced (listed but not purchasable). | [optional] 
**strike_price** | [**SodacardsDevpublicV1Money**](SodacardsDevpublicV1Money.md) | strike_price is an optional reference (pre-discount) price, in the currency of Money, for  display. Absent when there is none. | [optional] 
**bonus** | **str** | bonus describes any extra value granted with the item, e.g. \&quot;+10%\&quot;. Empty  when there is none. | [optional] 
**min_quantity** | **int** | min_quantity and max_quantity bound how many units an order line may buy. | [optional] 
**max_quantity** | **int** |  | [optional] 
**purchasable** | **bool** | purchasable is true when the item has a price and can be ordered now. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_product import SodacardsDevpublicV1Product

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1Product from a JSON string
sodacards_devpublic_v1_product_instance = SodacardsDevpublicV1Product.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1Product.to_json())

# convert the object into a dict
sodacards_devpublic_v1_product_dict = sodacards_devpublic_v1_product_instance.to_dict()
# create an instance of SodacardsDevpublicV1Product from a dict
sodacards_devpublic_v1_product_from_dict = SodacardsDevpublicV1Product.from_dict(sodacards_devpublic_v1_product_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


