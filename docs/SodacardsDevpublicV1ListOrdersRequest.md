# SodacardsDevpublicV1ListOrdersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**limit** | **int** | limit is the maximum number of orders to return (1..100). Zero applies the  default page size. | [optional] 
**cursor** | **str** | cursor is the next_cursor of the previous page. Empty for the first page. | [optional] 
**reference** | **str** | reference, when set, filters the list to the orders carrying that client  reference. The cursor is ignored when a reference is given. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_list_orders_request import SodacardsDevpublicV1ListOrdersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1ListOrdersRequest from a JSON string
sodacards_devpublic_v1_list_orders_request_instance = SodacardsDevpublicV1ListOrdersRequest.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1ListOrdersRequest.to_json())

# convert the object into a dict
sodacards_devpublic_v1_list_orders_request_dict = sodacards_devpublic_v1_list_orders_request_instance.to_dict()
# create an instance of SodacardsDevpublicV1ListOrdersRequest from a dict
sodacards_devpublic_v1_list_orders_request_from_dict = SodacardsDevpublicV1ListOrdersRequest.from_dict(sodacards_devpublic_v1_list_orders_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


