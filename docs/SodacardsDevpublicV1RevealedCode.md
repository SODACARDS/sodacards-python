# SodacardsDevpublicV1RevealedCode

RevealedCode is one delivered code of an order.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **str** | label names what the code is for (e.g. the product line). | [optional] 
**code** | **str** | code is the delivered value. Treat it as a secret: do not log it. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_revealed_code import SodacardsDevpublicV1RevealedCode

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1RevealedCode from a JSON string
sodacards_devpublic_v1_revealed_code_instance = SodacardsDevpublicV1RevealedCode.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1RevealedCode.to_json())

# convert the object into a dict
sodacards_devpublic_v1_revealed_code_dict = sodacards_devpublic_v1_revealed_code_instance.to_dict()
# create an instance of SodacardsDevpublicV1RevealedCode from a dict
sodacards_devpublic_v1_revealed_code_from_dict = SodacardsDevpublicV1RevealedCode.from_dict(sodacards_devpublic_v1_revealed_code_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


