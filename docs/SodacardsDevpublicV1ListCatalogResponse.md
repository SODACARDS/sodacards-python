# SodacardsDevpublicV1ListCatalogResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SodacardsDevpublicV1Product]**](SodacardsDevpublicV1Product.md) | data is the page of products, priced for the calling reseller. | [optional] 
**has_more** | **bool** | has_more is true when another page follows this one. | [optional] 
**next_cursor** | **str** | next_cursor fetches the next page. Empty on the last page. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_list_catalog_response import SodacardsDevpublicV1ListCatalogResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1ListCatalogResponse from a JSON string
sodacards_devpublic_v1_list_catalog_response_instance = SodacardsDevpublicV1ListCatalogResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1ListCatalogResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_list_catalog_response_dict = sodacards_devpublic_v1_list_catalog_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1ListCatalogResponse from a dict
sodacards_devpublic_v1_list_catalog_response_from_dict = SodacardsDevpublicV1ListCatalogResponse.from_dict(sodacards_devpublic_v1_list_catalog_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


