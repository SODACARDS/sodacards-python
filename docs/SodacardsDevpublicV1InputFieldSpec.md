# SodacardsDevpublicV1InputFieldSpec

InputFieldSpec describes one purchase-form field a product requires, so a  developer can build and validate an order line before placing it. Its value is  submitted on OrderLine.input_fields, keyed by this field's key.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **str** | key is the field&#39;s machine name and the key to use in  OrderLine.input_fields, e.g. \&quot;player_id\&quot;. | [optional] 
**type** | **str** | type is how to render and validate the value: \&quot;text\&quot;, \&quot;number\&quot; or \&quot;select\&quot;. | [optional] 
**required** | **bool** | required is true when an order line for this product must carry this field. | [optional] 
**regex** | **str** | regex, when present, is a regular expression the submitted value must match  (text and number fields). Empty when there is no pattern constraint. | [optional] 
**options** | [**List[SodacardsDevpublicV1InputFieldOption]**](SodacardsDevpublicV1InputFieldOption.md) | options are the allowed values of a \&quot;select\&quot; field, in display order. Empty  for text and number fields. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_input_field_spec import SodacardsDevpublicV1InputFieldSpec

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1InputFieldSpec from a JSON string
sodacards_devpublic_v1_input_field_spec_instance = SodacardsDevpublicV1InputFieldSpec.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1InputFieldSpec.to_json())

# convert the object into a dict
sodacards_devpublic_v1_input_field_spec_dict = sodacards_devpublic_v1_input_field_spec_instance.to_dict()
# create an instance of SodacardsDevpublicV1InputFieldSpec from a dict
sodacards_devpublic_v1_input_field_spec_from_dict = SodacardsDevpublicV1InputFieldSpec.from_dict(sodacards_devpublic_v1_input_field_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


