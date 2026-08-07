# SodacardsDevpublicV1Money

Money is an amount in a currency's minor units, together with the currency's  ISO-4217 code and its number of decimal places, so the amount can be  interpreted without assuming the currency. XOF (the West-African CFA franc) has  no minor unit, so an XOF amount is a whole franc value.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | [**Amount**](Amount.md) |  | [optional] 
**currency** | **str** | currency is the ISO-4217 code, e.g. \&quot;XOF\&quot;. | [optional] 
**minor_unit_exponent** | **int** | minor_unit_exponent is the currency&#39;s number of decimal places (0 for XOF,  2 for USD): amount divided by 10^minor_unit_exponent is the major-unit value. | [optional] 

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


