# SodacardsDevpublicV1GetProductResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product** | [**SodacardsDevpublicV1Product**](SodacardsDevpublicV1Product.md) | product is the requested product, priced for the reseller. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_get_product_response import SodacardsDevpublicV1GetProductResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1GetProductResponse from a JSON string
sodacards_devpublic_v1_get_product_response_instance = SodacardsDevpublicV1GetProductResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1GetProductResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_get_product_response_dict = sodacards_devpublic_v1_get_product_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1GetProductResponse from a dict
sodacards_devpublic_v1_get_product_response_from_dict = SodacardsDevpublicV1GetProductResponse.from_dict(sodacards_devpublic_v1_get_product_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


