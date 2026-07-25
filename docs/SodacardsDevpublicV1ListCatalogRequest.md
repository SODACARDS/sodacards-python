# SodacardsDevpublicV1ListCatalogRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**limit** | **int** | limit is the maximum number of products to return (1..100). Zero applies the  default page size. | [optional] 
**cursor** | **str** | cursor is the next_cursor of the previous page. Empty for the first page. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_list_catalog_request import SodacardsDevpublicV1ListCatalogRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1ListCatalogRequest from a JSON string
sodacards_devpublic_v1_list_catalog_request_instance = SodacardsDevpublicV1ListCatalogRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1ListCatalogRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_list_catalog_request_dict = sodacards_devpublic_v1_list_catalog_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1ListCatalogRequest from a dict
sodacards_devpublic_v1_list_catalog_request_from_dict = SodacardsDevpublicV1ListCatalogRequest.from_dict(sodacards_devpublic_v1_list_catalog_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


