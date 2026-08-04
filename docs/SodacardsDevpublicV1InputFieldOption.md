# SodacardsDevpublicV1InputFieldOption

InputFieldOption is one allowed value of a \"select\" input field.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** | value is what to submit on OrderLine.input_fields for this option. | [optional] 
**label** | **str** | label is the human-readable display for the option. | [optional] 
**parent_value** | **str** | parent_value gates a cascading option: the value of the parent field&#39;s option  that must be selected for this option to apply (e.g. a server option gated by  the chosen region). Empty when the option is not part of a cascade. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_input_field_option import SodacardsDevpublicV1InputFieldOption

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1InputFieldOption from a JSON string
sodacards_devpublic_v1_input_field_option_instance = SodacardsDevpublicV1InputFieldOption.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1InputFieldOption.to_json())

# convert the object into a dict
sodacards_devpublic_v1_input_field_option_dict = sodacards_devpublic_v1_input_field_option_instance.to_dict()
# create an instance of SodacardsDevpublicV1InputFieldOption from a dict
sodacards_devpublic_v1_input_field_option_from_dict = SodacardsDevpublicV1InputFieldOption.from_dict(sodacards_devpublic_v1_input_field_option_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


