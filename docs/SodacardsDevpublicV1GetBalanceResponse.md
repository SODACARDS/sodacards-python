# SodacardsDevpublicV1GetBalanceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**balance** | [**SodacardsDevpublicV1Money**](SodacardsDevpublicV1Money.md) | balance is the reseller&#39;s prepaid wallet balance. For a test key it is a  fixed sandbox value, clearly not the production wallet. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_get_balance_response import SodacardsDevpublicV1GetBalanceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1GetBalanceResponse from a JSON string
sodacards_devpublic_v1_get_balance_response_instance = SodacardsDevpublicV1GetBalanceResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1GetBalanceResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_get_balance_response_dict = sodacards_devpublic_v1_get_balance_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1GetBalanceResponse from a dict
sodacards_devpublic_v1_get_balance_response_from_dict = SodacardsDevpublicV1GetBalanceResponse.from_dict(sodacards_devpublic_v1_get_balance_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


