# SodacardsDevpublicV1RevealOrderCodesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**codes** | [**List[SodacardsDevpublicV1RevealedCode]**](SodacardsDevpublicV1RevealedCode.md) | codes are the delivered codes of the order. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_reveal_order_codes_response import SodacardsDevpublicV1RevealOrderCodesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1RevealOrderCodesResponse from a JSON string
sodacards_devpublic_v1_reveal_order_codes_response_instance = SodacardsDevpublicV1RevealOrderCodesResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1RevealOrderCodesResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_reveal_order_codes_response_dict = sodacards_devpublic_v1_reveal_order_codes_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1RevealOrderCodesResponse from a dict
sodacards_devpublic_v1_reveal_order_codes_response_from_dict = SodacardsDevpublicV1RevealOrderCodesResponse.from_dict(sodacards_devpublic_v1_reveal_order_codes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


