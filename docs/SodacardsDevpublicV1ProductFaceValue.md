# SodacardsDevpublicV1ProductFaceValue

ProductFaceValue is the nominal value printed on a product. amount is a decimal  string (e.g. \"10.00\") so fractional face values are exact.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** | amount is the face value as an exact decimal string, e.g. \&quot;10.00\&quot;. | [optional] 
**currency** | **str** | currency is the ISO-4217 code of the face value, e.g. \&quot;USD\&quot;. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_product_face_value import SodacardsDevpublicV1ProductFaceValue

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1ProductFaceValue from a JSON string
sodacards_devpublic_v1_product_face_value_instance = SodacardsDevpublicV1ProductFaceValue.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1ProductFaceValue.to_json())

# convert the object into a dict
sodacards_devpublic_v1_product_face_value_dict = sodacards_devpublic_v1_product_face_value_instance.to_dict()
# create an instance of SodacardsDevpublicV1ProductFaceValue from a dict
sodacards_devpublic_v1_product_face_value_from_dict = SodacardsDevpublicV1ProductFaceValue.from_dict(sodacards_devpublic_v1_product_face_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


