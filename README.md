# SODACARDS Python SDK

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)
[![Docs](https://img.shields.io/badge/docs-developer.sodacards.com-003087.svg)](https://developer.sodacards.com)

The official Python client for the [SODACARDS Developer API](https://developer.sodacards.com) — sell gift cards and game top-ups from your own systems, across West Africa.

Browse the catalog, place orders, retrieve delivered codes, and subscribe to webhooks, all with type-checked models.

## Requirements

Python 3.10 or newer.

## Installation

```sh
pip install sodacards
```

## Authentication

Every request is authenticated with an API key that you generate from the [developer dashboard](https://developer.sodacards.com). Keys are prefixed `sc_live_` (production) or `sc_test_` (sandbox); the sandbox returns fake codes so you can integrate safely.

Load the key from the environment — never hard-code it in source.

```python
import os
import sodacards

configuration = sodacards.Configuration(host="https://api.sodacards.com")
configuration.api_key["ApiKeyAuth"] = os.environ["SODACARDS_API_KEY"]
```

## Quickstart

```python
import os
import sodacards
from sodacards.models import (
    SodacardsDevpublicV1PlaceOrderRequest,
    SodacardsDevpublicV1OrderLine,
)

configuration = sodacards.Configuration(host="https://api.sodacards.com")
configuration.api_key["ApiKeyAuth"] = os.environ["SODACARDS_API_KEY"]

with sodacards.ApiClient(configuration) as api_client:
    api = sodacards.DefaultApi(api_client)

    # 1. Discover what you can sell.
    catalog = api.list_catalog()

    # 2. Place an order for one product.
    order = api.place_order(
        SodacardsDevpublicV1PlaceOrderRequest(
            lines=[SodacardsDevpublicV1OrderLine(product_id="prod_123", quantity=1)],
            reference="my-internal-ref-0001",
        )
    )

    # 3. Read back the delivered codes once the order is fulfilled.
    codes = api.reveal_order_codes(order.order.id)
    print(codes)
```

## Idempotency

`place_order` is the only state-changing call. Send an `Idempotency-Key` header so a retried request never creates a duplicate order — the API returns the original order for a repeated key.

```python
api.place_order(request, _headers={"Idempotency-Key": "a-unique-key-per-order"})
```

## Operations

| Method | Description |
| --- | --- |
| `list_catalog` | List sellable products (cursor-paginated). |
| `get_product` | Fetch a single product by id. |
| `place_order` | Buy one or more products. |
| `get_order` | Retrieve an order by id. |
| `list_orders` | List your orders (cursor-paginated). |
| `reveal_order_codes` | Reveal the delivered codes for a fulfilled order. |
| `register_webhook` | Subscribe an endpoint to events. |
| `list_webhooks` | List your webhook endpoints. |
| `delete_webhook` | Remove a webhook endpoint. |
| `ping` | Health check for your credentials. |

## Pagination

List endpoints use cursor (keyset) pagination. Pass the `next_cursor` returned by a response as the `cursor` argument of the next call until it is empty.

## Errors

Failed requests raise `sodacards.rest.ApiException`, which carries the HTTP status and the API error body.

## Documentation and support

- API reference and guides: <https://developer.sodacards.com>
- Support: <mailto:support@sodacards.com>

## License

Released under the [MIT License](./LICENSE).

---

This SDK is generated from the SODACARDS OpenAPI specification and is regenerated automatically whenever the API changes. Open issues on the [documentation portal](https://developer.sodacards.com) rather than editing generated files directly.
