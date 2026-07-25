# sodacards.DefaultApi

All URIs are relative to *https://api.sodacards.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_webhook**](DefaultApi.md#delete_webhook) | **DELETE** /v1/webhooks/{id} | DeleteWebhook
[**get_order**](DefaultApi.md#get_order) | **GET** /v1/orders/{id} | GetOrder
[**get_product**](DefaultApi.md#get_product) | **GET** /v1/products/{id} | GetProduct
[**list_catalog**](DefaultApi.md#list_catalog) | **GET** /v1/catalog | ListCatalog
[**list_orders**](DefaultApi.md#list_orders) | **GET** /v1/orders | ListOrders
[**list_webhooks**](DefaultApi.md#list_webhooks) | **GET** /v1/webhooks | ListWebhooks
[**ping**](DefaultApi.md#ping) | **GET** /v1/ping | Ping
[**place_order**](DefaultApi.md#place_order) | **POST** /v1/orders | PlaceOrder
[**register_webhook**](DefaultApi.md#register_webhook) | **POST** /v1/webhooks | RegisterWebhook
[**reveal_order_codes**](DefaultApi.md#reveal_order_codes) | **GET** /v1/orders/{order_id}/codes | RevealOrderCodes


# **delete_webhook**
> object delete_webhook(id)

DeleteWebhook

DeleteWebhook removes a webhook endpoint.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
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
    api_instance = sodacards.DefaultApi(api_client)
    id = 'id_example' # str | id is the webhook endpoint to remove.

    try:
        # DeleteWebhook
        api_response = api_instance.delete_webhook(id)
        print("The response of DefaultApi->delete_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id is the webhook endpoint to remove. | 

### Return type

**object**

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

# **get_order**
> SodacardsDevpublicV1GetOrderResponse get_order(id)

GetOrder

GetOrder returns one of the reseller's orders by id, with its lines and
 current status. A live key reads live orders and a test key reads its own
 sandbox orders; an id that is not the caller's is reported as not found.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_get_order_response import SodacardsDevpublicV1GetOrderResponse
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
    api_instance = sodacards.DefaultApi(api_client)
    id = 'id_example' # str | id is the order id, from PlaceOrder.

    try:
        # GetOrder
        api_response = api_instance.get_order(id)
        print("The response of DefaultApi->get_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id is the order id, from PlaceOrder. | 

### Return type

[**SodacardsDevpublicV1GetOrderResponse**](SodacardsDevpublicV1GetOrderResponse.md)

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

# **get_product**
> SodacardsDevpublicV1GetProductResponse get_product(id)

GetProduct

GetProduct returns a single product by its id, priced for the reseller. The
 id is the one carried by a catalog entry. A product the reseller may not see
 (unlisted, hidden or inactive) is reported as not found, so an id cannot be
 probed to learn what exists outside the reseller's catalog.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_get_product_response import SodacardsDevpublicV1GetProductResponse
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
    api_instance = sodacards.DefaultApi(api_client)
    id = 'id_example' # str | id is the product id, taken from a catalog entry.

    try:
        # GetProduct
        api_response = api_instance.get_product(id)
        print("The response of DefaultApi->get_product:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_product: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id is the product id, taken from a catalog entry. | 

### Return type

[**SodacardsDevpublicV1GetProductResponse**](SodacardsDevpublicV1GetProductResponse.md)

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

# **list_catalog**
> SodacardsDevpublicV1ListCatalogResponse list_catalog(limit=limit, cursor=cursor)

ListCatalog

ListCatalog returns a page of the products the reseller may sell, each with
 the reseller's price. It is cursor-paginated: pass next_cursor from the
 previous page to fetch the next. A product's id is the identifier used to
 order it.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_list_catalog_response import SodacardsDevpublicV1ListCatalogResponse
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
    api_instance = sodacards.DefaultApi(api_client)
    limit = 56 # int | limit is the maximum number of products to return (1..100). Zero applies the  default page size. (optional)
    cursor = 'cursor_example' # str | cursor is the next_cursor of the previous page. Empty for the first page. (optional)

    try:
        # ListCatalog
        api_response = api_instance.list_catalog(limit=limit, cursor=cursor)
        print("The response of DefaultApi->list_catalog:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_catalog: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| limit is the maximum number of products to return (1..100). Zero applies the  default page size. | [optional] 
 **cursor** | **str**| cursor is the next_cursor of the previous page. Empty for the first page. | [optional] 

### Return type

[**SodacardsDevpublicV1ListCatalogResponse**](SodacardsDevpublicV1ListCatalogResponse.md)

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

# **list_orders**
> SodacardsDevpublicV1ListOrdersResponse list_orders(limit=limit, cursor=cursor, reference=reference)

ListOrders

ListOrders returns a page of the reseller's orders, newest first. It is
 cursor-paginated: pass next_cursor from the previous page to fetch the next.
 A live key lists live orders and a test key lists its own sandbox orders.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_list_orders_response import SodacardsDevpublicV1ListOrdersResponse
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
    api_instance = sodacards.DefaultApi(api_client)
    limit = 56 # int | limit is the maximum number of orders to return (1..100). Zero applies the  default page size. (optional)
    cursor = 'cursor_example' # str | cursor is the next_cursor of the previous page. Empty for the first page. (optional)
    reference = 'reference_example' # str | reference, when set, filters the list to the orders carrying that client  reference. The cursor is ignored when a reference is given. (optional)

    try:
        # ListOrders
        api_response = api_instance.list_orders(limit=limit, cursor=cursor, reference=reference)
        print("The response of DefaultApi->list_orders:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_orders: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| limit is the maximum number of orders to return (1..100). Zero applies the  default page size. | [optional] 
 **cursor** | **str**| cursor is the next_cursor of the previous page. Empty for the first page. | [optional] 
 **reference** | **str**| reference, when set, filters the list to the orders carrying that client  reference. The cursor is ignored when a reference is given. | [optional] 

### Return type

[**SodacardsDevpublicV1ListOrdersResponse**](SodacardsDevpublicV1ListOrdersResponse.md)

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

# **list_webhooks**
> SodacardsDevpublicV1ListWebhooksResponse list_webhooks()

ListWebhooks

ListWebhooks returns the reseller's registered webhook endpoints. It never
 returns their signing secrets.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_list_webhooks_response import SodacardsDevpublicV1ListWebhooksResponse
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
    api_instance = sodacards.DefaultApi(api_client)

    try:
        # ListWebhooks
        api_response = api_instance.list_webhooks()
        print("The response of DefaultApi->list_webhooks:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_webhooks: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SodacardsDevpublicV1ListWebhooksResponse**](SodacardsDevpublicV1ListWebhooksResponse.md)

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

# **ping**
> SodacardsDevpublicV1PingResponse ping()

Ping

Ping confirms a key works and reports which reseller and environment it
 authenticated as. It is the health check a developer hits first.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_ping_response import SodacardsDevpublicV1PingResponse
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
    api_instance = sodacards.DefaultApi(api_client)

    try:
        # Ping
        api_response = api_instance.ping()
        print("The response of DefaultApi->ping:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->ping: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SodacardsDevpublicV1PingResponse**](SodacardsDevpublicV1PingResponse.md)

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

# **place_order**
> SodacardsDevpublicV1PlaceOrderResponse place_order(sodacards_devpublic_v1_place_order_request)

PlaceOrder

PlaceOrder buys one or more products, settled from the reseller's prepaid
 wallet. It is asynchronous: the order is accepted and fulfilled in the
 background, so the response carries the order id and a status to poll. The
 request MUST carry an Idempotency-Key header, so a retried request never
 places a second order.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_place_order_request import SodacardsDevpublicV1PlaceOrderRequest
from sodacards.models.sodacards_devpublic_v1_place_order_response import SodacardsDevpublicV1PlaceOrderResponse
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
    api_instance = sodacards.DefaultApi(api_client)
    sodacards_devpublic_v1_place_order_request = sodacards.SodacardsDevpublicV1PlaceOrderRequest() # SodacardsDevpublicV1PlaceOrderRequest | 

    try:
        # PlaceOrder
        api_response = api_instance.place_order(sodacards_devpublic_v1_place_order_request)
        print("The response of DefaultApi->place_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->place_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sodacards_devpublic_v1_place_order_request** | [**SodacardsDevpublicV1PlaceOrderRequest**](SodacardsDevpublicV1PlaceOrderRequest.md)|  | 

### Return type

[**SodacardsDevpublicV1PlaceOrderResponse**](SodacardsDevpublicV1PlaceOrderResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **register_webhook**
> SodacardsDevpublicV1RegisterWebhookResponse register_webhook(sodacards_devpublic_v1_register_webhook_request)

RegisterWebhook

RegisterWebhook registers a URL to receive signed event deliveries. The URL
 must be HTTPS and publicly routable. The response carries the signing secret
 once; store it, as it is never shown again.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_register_webhook_request import SodacardsDevpublicV1RegisterWebhookRequest
from sodacards.models.sodacards_devpublic_v1_register_webhook_response import SodacardsDevpublicV1RegisterWebhookResponse
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
    api_instance = sodacards.DefaultApi(api_client)
    sodacards_devpublic_v1_register_webhook_request = sodacards.SodacardsDevpublicV1RegisterWebhookRequest() # SodacardsDevpublicV1RegisterWebhookRequest | 

    try:
        # RegisterWebhook
        api_response = api_instance.register_webhook(sodacards_devpublic_v1_register_webhook_request)
        print("The response of DefaultApi->register_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->register_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sodacards_devpublic_v1_register_webhook_request** | [**SodacardsDevpublicV1RegisterWebhookRequest**](SodacardsDevpublicV1RegisterWebhookRequest.md)|  | 

### Return type

[**SodacardsDevpublicV1RegisterWebhookResponse**](SodacardsDevpublicV1RegisterWebhookResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reveal_order_codes**
> SodacardsDevpublicV1RevealOrderCodesResponse reveal_order_codes(order_id)

RevealOrderCodes

RevealOrderCodes returns the delivered codes of a completed order. Codes are
 available once the order is completed; a still-processing order reports that
 it is not ready. Reveals are rate-limited per order.

### Example

* Api Key Authentication (ApiKeyAuth):

```python
import sodacards
from sodacards.models.sodacards_devpublic_v1_reveal_order_codes_response import SodacardsDevpublicV1RevealOrderCodesResponse
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
    api_instance = sodacards.DefaultApi(api_client)
    order_id = 'order_id_example' # str | order_id is the order whose codes to reveal.

    try:
        # RevealOrderCodes
        api_response = api_instance.reveal_order_codes(order_id)
        print("The response of DefaultApi->reveal_order_codes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->reveal_order_codes: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **str**| order_id is the order whose codes to reveal. | 

### Return type

[**SodacardsDevpublicV1RevealOrderCodesResponse**](SodacardsDevpublicV1RevealOrderCodesResponse.md)

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

