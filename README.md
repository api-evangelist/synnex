# Synnex (TD SYNNEX)

SYNNEX Corporation (now TD SYNNEX) is a Fortune 100 global IT distribution company and solutions aggregator that connects technology vendors with resellers, system integrators, and enterprise customers. TD SYNNEX was formed in 2021 through the merger of Synnex Corporation and Tech Data.

**Type:** Company (Fortune 100)
**Website:** [tdsynnex.com](https://www.tdsynnex.com)
**API Documentation:** [docs.streamone.cloud](https://docs.streamone.cloud/)

## APIs

### StreamOne ION API

The StreamOne ION API is TD SYNNEX's interface for cloud vendors and reseller partners to manage cloud subscriptions, product catalogs, end customers, and orders. Uses OAuth 2.0 authentication and supports multi-vendor cloud marketplace operations.

- **Documentation:** [docs.streamone.cloud](https://docs.streamone.cloud/)
- **OpenAPI:** [openapi/synnex-streamone-ion-openapi.yml](openapi/synnex-streamone-ion-openapi.yml)
- **Base URL:** `https://ion.tdsynnex.com/api/v3`

| Method | Path | Summary |
|--------|------|---------|
| GET | /accounts/{accountId}/customers | List Customers |
| POST | /accounts/{accountId}/customers | Create Customer |
| GET | /accounts/{accountId}/customers/{customerId} | Get Customer |
| PUT | /accounts/{accountId}/customers/{customerId} | Update Customer |
| GET | /accounts/{accountId}/products | List Products |
| GET | /accounts/{accountId}/products/{productId} | Get Product |
| GET | /accounts/{accountId}/orders | List Orders |
| POST | /accounts/{accountId}/orders | Create Order |
| GET | /accounts/{accountId}/orders/{orderId} | Get Order |
| GET | /accounts/{accountId}/customers/{customerId}/subscriptions | List Subscriptions |
| GET | /accounts/{accountId}/customers/{customerId}/subscriptions/{subscriptionId} | Get Subscription |
| PUT | /accounts/{accountId}/customers/{customerId}/subscriptions/{subscriptionId} | Update Subscription |
| POST | /accounts/{accountId}/cart | Create Cart |
| POST | /accounts/{accountId}/cart/{cartId}/checkout | Checkout Cart |
| GET | /accounts/{accountId}/reports | List Reports |

### Digital Bridge API

The Digital Bridge Developer Portal gives engineering teams direct access to REST APIs for products, pricing, orders, renewals, and cloud services.

- **Documentation:** [tdsynnex.com/na/us/digital-bridge](https://www.tdsynnex.com/na/us/digital-bridge/)

## Naftiko Capabilities

### Shared Definitions

| File | Description |
|------|-------------|
| [capabilities/shared/streamone-ion.yaml](capabilities/shared/streamone-ion.yaml) | StreamOne ION API consumed definition |

### Workflow Capabilities

| Capability | Description | Tools |
|-----------|-------------|-------|
| [cloud-marketplace.yaml](capabilities/cloud-marketplace.yaml) | Unified cloud marketplace operations (customers + products + orders + subscriptions + reports) | 7 tools |

## Artifacts

| Type | File |
|------|------|
| OpenAPI | [openapi/synnex-streamone-ion-openapi.yml](openapi/synnex-streamone-ion-openapi.yml) |
| Spectral Rules | [rules/synnex-rules.yml](rules/synnex-rules.yml) |
| JSON Schema | [json-schema/synnex-customer-schema.json](json-schema/synnex-customer-schema.json) |
| JSON Schema | [json-schema/synnex-subscription-schema.json](json-schema/synnex-subscription-schema.json) |
| JSON Structure | [json-structure/synnex-subscription-structure.json](json-structure/synnex-subscription-structure.json) |
| JSON-LD Context | [json-ld/synnex-context.jsonld](json-ld/synnex-context.jsonld) |
| Vocabulary | [vocabulary/synnex-vocabulary.yml](vocabulary/synnex-vocabulary.yml) |

## Examples

| File | Description |
|------|-------------|
| [examples/synnex-streamone-ion-listCustomers-example.json](examples/synnex-streamone-ion-listCustomers-example.json) | List customers response |
| [examples/synnex-streamone-ion-createOrder-example.json](examples/synnex-streamone-ion-createOrder-example.json) | Create order request/response |

## Features

- OAuth 2.0 Authentication
- End Customer Management
- Multi-Vendor Product Catalog
- Order Management
- Subscription Lifecycle Management (suspend, reactivate, upgrade)
- Shopping Cart Operations
- Cloud Provider Account Management
- Reporting and Data Export (JSON/CSV)
- Swagger/OpenAPI Testing Interface
- Sandbox Environment
- Multi-Currency and Multi-Language Support

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
