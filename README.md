# CurrencyAPI (currencyapi)

CurrencyAPI (currencyapi.com, an Everapi product) is a foreign exchange rate and currency conversion REST API delivering real-time and historical exchange rates for fiat currencies, precious metals, and cryptocurrencies. A single versioned API (base `https://api.currencyapi.com/v3`) covers latest rates, historical rates back to 1999, time-series ranges down to minute accuracy, value conversion, currency metadata, and account quota status.

The API is fully documented and publicly accessible: sign up on currencyapi.com, get an API key, and authenticate by sending it as an `apikey` HTTP header (recommended) or `apikey` query parameter. A free-forever plan includes 300 requests per month with daily rate updates and a 10 requests/minute limit; paid plans ($9.99 to $79.99 per month, plus a custom enterprise tier) raise the monthly quota to 15,000-1,700,000+ requests, refresh rates as often as every 60 seconds, and unlock commercial use, the convert endpoint (Small and up), and the range endpoint (Medium and up). Only successful calls count against your quota. There is no public WebSocket or streaming API - all access is request/response REST over HTTPS.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/apis.yml)

## Tags

- Foreign Exchange
- Currency
- Exchange Rates
- FX
- Currency Conversion
- Financial Data

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

### CurrencyAPI Latest Exchange Rates API

Returns the latest foreign exchange rates for any base currency against all or selected quote currencies, filterable by type (fiat, metal, crypto). Rates refresh from daily on the free plan down to every 60 seconds on paid plans.

- **Human URL:** [https://currencyapi.com/docs/latest](https://currencyapi.com/docs/latest)
- **Base URL:** `https://api.currencyapi.com/v3`

#### Tags

- Foreign Exchange
- Exchange Rates
- Real-Time
- FX

#### Properties

- [Documentation](https://currencyapi.com/docs/latest)
- [OpenAPI](openapi/currencyapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/currencyapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/currencyapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CurrencyAPI Historical Exchange Rates API

Retrieves end-of-day foreign exchange rates for a specific date, with historical FX data reaching back to 1999, for any base currency and optional currency or type filters.

- **Human URL:** [https://currencyapi.com/docs/historical](https://currencyapi.com/docs/historical)
- **Base URL:** `https://api.currencyapi.com/v3`

#### Tags

- Foreign Exchange
- Exchange Rates
- Historical Data
- FX

#### Properties

- [Documentation](https://currencyapi.com/docs/historical)
- [OpenAPI](openapi/currencyapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/currencyapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/currencyapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CurrencyAPI Range Exchange Rates API

Returns time-series exchange rate data between a start and end datetime in one call, with selectable accuracy of day (up to 366 days), hour, quarter hour, or minute for charting and FX analytics. Available on the Medium plan and above.

- **Human URL:** [https://currencyapi.com/docs/range](https://currencyapi.com/docs/range)
- **Base URL:** `https://api.currencyapi.com/v3`

#### Tags

- Foreign Exchange
- Time Series
- Exchange Rates
- FX

#### Properties

- [Documentation](https://currencyapi.com/docs/range)
- [OpenAPI](openapi/currencyapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/currencyapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/currencyapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CurrencyAPI Convert API

Converts any monetary value from a base currency into one or more target currencies using either today's exchange rates or the rates of a given historical date. Available on paid plans (Small and up).

- **Human URL:** [https://currencyapi.com/docs/convert](https://currencyapi.com/docs/convert)
- **Base URL:** `https://api.currencyapi.com/v3`

#### Tags

- Currency Conversion
- Foreign Exchange
- FX

#### Properties

- [Documentation](https://currencyapi.com/docs/convert)
- [OpenAPI](openapi/currencyapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/currencyapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/currencyapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CurrencyAPI Currencies API

Lists all supported currencies with metadata - symbol, name, native symbol, decimal digits, rounding, plural name, type (fiat, metal, crypto), and associated countries - filterable by code or type.

- **Human URL:** [https://currencyapi.com/docs/currencies](https://currencyapi.com/docs/currencies)
- **Base URL:** `https://api.currencyapi.com/v3`

#### Tags

- Currency
- Reference Data
- Metadata

#### Properties

- [Documentation](https://currencyapi.com/docs/currencies)
- [OpenAPI](openapi/currencyapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/currencyapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/currencyapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CurrencyAPI Status API

Programmatically checks whether the API is up and returns your monthly and grace quota usage. Requests to this endpoint do not count against your quota or rate limit.

- **Human URL:** [https://currencyapi.com/docs/status](https://currencyapi.com/docs/status)
- **Base URL:** `https://api.currencyapi.com/v3`

#### Tags

- Status
- Quota
- Account

#### Properties

- [Documentation](https://currencyapi.com/docs/status)
- [OpenAPI](openapi/currencyapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/currencyapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/currencyapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/everapihq)
- [LinkedIn](https://www.linkedin.com/company/everapi)
- [Website](https://currencyapi.com)
- [Documentation](https://currencyapi.com/docs)
- [API Reference](https://currencyapi.com/docs/latest)
- [Authentication](https://currencyapi.com/docs/authentication)
- [Pricing](https://currencyapi.com/pricing)
- [Plans](plans/currencyapi-plans-pricing.yml)
- [Rate Limits](rate-limits/currencyapi-rate-limits.yml)
- [Fin Ops](finops/currencyapi-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
