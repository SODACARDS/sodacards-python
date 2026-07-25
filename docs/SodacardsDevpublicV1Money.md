# SodacardsDevpublicV1Money

Money is an amount in the currency's minor units together with its ISO-4217  code. XOF (the West-African CFA franc) has no minor unit, so for XOF amount is  the whole franc value.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | [**Amount**](Amount.md) |  | [optional] 
**currency** | **str** | currency is the ISO-4217 code, e.g. \&quot;XOF\&quot;. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_money import SodacardsDevpublicV1Money

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1Money from a JSON string
sodacards_devpublic_v1_money_instance = SodacardsDevpublicV1Money.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1Money.to_json())

# convert the object into a dict
sodacards_devpublic_v1_money_dict = sodacards_devpublic_v1_money_instance.to_dict()
# create an instance of SodacardsDevpublicV1Money from a dict
sodacards_devpublic_v1_money_from_dict = SodacardsDevpublicV1Money.from_dict(sodacards_devpublic_v1_money_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


