# CurrencyAPI (currencyapi)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
