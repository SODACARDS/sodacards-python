# sodacards.PublicAPIServiceApi

All URIs are relative to *https://api.sodacards.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**public_api_service_get_balance**](PublicAPIServiceApi.md#public_api_service_get_balance) | **GET** /v1/balance | GetBalance
[**public_api_service_rotate_webhook_secret**](PublicAPIServiceApi.md#public_api_service_rotate_webhook_secret) | **POST** /v1/webhooks/{id}/rotate | RotateWebhookSecret


# **public_api_service_get_balance**
> SodacardsDevpublicV1GetBalanceResponse public_api_service_get_balance()

GetBalance

GetBalance returns the reseller's prepaid wallet balance, the same funds a
 live order is settled from. It reads only the caller's own wallet. A test key
 reads a fixed sandbox balance, never the real one, so a test integration can
 exercise the read without seeing production funds.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_get_balance_response import SodacardsDevpublicV1GetBalanceResponse
from sodacards.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sodacards.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sodacards.Configuration(
    host = "https://api.sodacards.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with sodacards.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sodacards.PublicAPIServiceApi(api_client)

    try:
        # GetBalance
        api_response = api_instance.public_api_service_get_balance()
        print("The response of PublicAPIServiceApi->public_api_service_get_balance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicAPIServiceApi->public_api_service_get_balance: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SodacardsDevpublicV1GetBalanceResponse**](SodacardsDevpublicV1GetBalanceResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **public_api_service_rotate_webhook_secret**
> SodacardsDevpublicV1RotateWebhookSecretResponse public_api_service_rotate_webhook_secret(id)

RotateWebhookSecret

RotateWebhookSecret issues a new signing secret for an endpoint without
 interrupting deliveries: the new secret is returned once, and the previous one
 stays valid until prev_secret_expires_at. During that window deliveries are
 signed with both, so switch your verification to the new secret before the
 deadline. Rotating again replaces the outgoing secret rather than adding a
 third, so at most two secrets are ever accepted at once.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_rotate_webhook_secret_response import SodacardsDevpublicV1RotateWebhookSecretResponse
from sodacards.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sodacards.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sodacards.Configuration(
    host = "https://api.sodacards.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with sodacards.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sodacards.PublicAPIServiceApi(api_client)
    id = 'id_example' # str | id is the webhook endpoint whose signing secret to rotate.

    try:
        # RotateWebhookSecret
        api_response = api_instance.public_api_service_rotate_webhook_secret(id)
        print("The response of PublicAPIServiceApi->public_api_service_rotate_webhook_secret:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicAPIServiceApi->public_api_service_rotate_webhook_secret: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id is the webhook endpoint whose signing secret to rotate. | 

### Return type

[**SodacardsDevpublicV1RotateWebhookSecretResponse**](SodacardsDevpublicV1RotateWebhookSecretResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

