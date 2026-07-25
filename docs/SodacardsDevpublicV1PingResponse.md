# SodacardsDevpublicV1PingResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** | status is \&quot;ok\&quot; when the key authenticated. | [optional] 
**environment** | **str** | environment is \&quot;live\&quot; or \&quot;test\&quot;, so a developer sees which mode their key is  in. | [optional] 
**reseller_id** | **str** | reseller_id is the account the key belongs to. | [optional] 

## Example

```python
from sodacards.models.sodacards_devpublic_v1_ping_response import SodacardsDevpublicV1PingResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SodacardsDevpublicV1PingResponse from a JSON string
sodacards_devpublic_v1_ping_response_instance = SodacardsDevpublicV1PingResponse.from_json(json)
# print the JSON string representation of the object
print(SodacardsDevpublicV1PingResponse.to_json())

# convert the object into a dict
sodacards_devpublic_v1_ping_response_dict = sodacards_devpublic_v1_ping_response_instance.to_dict()
# create an instance of SodacardsDevpublicV1PingResponse from a dict
sodacards_devpublic_v1_ping_response_from_dict = SodacardsDevpublicV1PingResponse.from_dict(sodacards_devpublic_v1_ping_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


