# SodacardsDevpublicV1GetProductRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | id is the product id, taken from a catalog entry. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_get_product_request import SodacardsDevpublicV1GetProductRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1GetProductRequest from a JSON string
sodacards_devpublic_v1_get_product_request_instance = SodacardsDevpublicV1GetProductRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1GetProductRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_get_product_request_dict = sodacards_devpublic_v1_get_product_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1GetProductRequest from a dict
sodacards_devpublic_v1_get_product_request_from_dict = SodacardsDevpublicV1GetProductRequest.from_dict(sodacards_devpublic_v1_get_product_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


