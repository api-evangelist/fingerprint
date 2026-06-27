# Fingerprint (fingerprint)

Fingerprint (formerly FingerprintJS) is a device-identification and fraud-prevention platform. Its browser and mobile agents generate a stable visitorId, and the Server API returns detailed identification events enriched with Smart Signals (bot, VPN, proxy, tampering, emulator, and more) for account takeover, payment fraud, and bot-mitigation use cases.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/fingerprint/refs/heads/main/apis.yml)

## Tags

- Device Identification
- Fraud Prevention
- Bot Detection
- Smart Signals
- Identity

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### Fingerprint Events API

Retrieve and update the complete identification event for a single requestId, including device attributes and all enabled Smart Signals. Authenticated with the Auth-API-Key header.

- **Human URL:** [https://dev.fingerprint.com/reference/getevent](https://dev.fingerprint.com/reference/getevent)
- **Base URL:** `https://api.fpjs.io`

#### Tags

- Events
- Identification
- Smart Signals

#### Properties

- [Documentation](https://dev.fingerprint.com/docs/server-api)
- [API Reference](https://dev.fingerprint.com/reference/getevent)
- [OpenAPI](openapi/fingerprint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fingerprint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fingerprint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fingerprint Events Search API

Query identification events for a workspace using a wide range of filters - visitorId, linkedId, bot, IP address, time range, suspect, and individual Smart Signal flags - with cursor pagination.

- **Human URL:** [https://dev.fingerprint.com/reference/searchevents](https://dev.fingerprint.com/reference/searchevents)
- **Base URL:** `https://api.fpjs.io`

#### Tags

- Events
- Search
- Filtering

#### Properties

- [API Reference](https://dev.fingerprint.com/reference/searchevents)
- [OpenAPI](openapi/fingerprint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fingerprint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fingerprint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fingerprint Visitors API

Retrieve the visit history for a given visitorId with pagination and time-range filtering, and delete all data associated with a visitorId for privacy and data-subject requests.

- **Human URL:** [https://dev.fingerprint.com/reference/getvisits](https://dev.fingerprint.com/reference/getvisits)
- **Base URL:** `https://api.fpjs.io`

#### Tags

- Visitors
- History
- Identity

#### Properties

- [API Reference](https://dev.fingerprint.com/reference/getvisits)
- [OpenAPI](openapi/fingerprint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fingerprint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fingerprint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fingerprint Related Visitors API

Find other visitorIds that likely belong to the same person across browsers and incognito sessions, supporting linked-identity and account-sharing detection.

- **Human URL:** [https://dev.fingerprint.com/reference/getrelatedvisitors](https://dev.fingerprint.com/reference/getrelatedvisitors)
- **Base URL:** `https://api.fpjs.io`

#### Tags

- Related Visitors
- Linking
- Identity

#### Properties

- [API Reference](https://dev.fingerprint.com/reference/getrelatedvisitors)
- [OpenAPI](openapi/fingerprint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fingerprint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fingerprint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fingerprint Smart Signals API

Risk signals returned inside identification events - bot detection, VPN, proxy, Tor, IP blocklist, tampering, virtual machine, incognito, emulator, root, jailbreak, Frida, cloned app, factory reset, and velocity - for fraud and abuse decisioning.

- **Human URL:** [https://dev.fingerprint.com/docs/smart-signals-overview](https://dev.fingerprint.com/docs/smart-signals-overview)
- **Base URL:** `https://api.fpjs.io`

#### Tags

- Smart Signals
- Bot Detection
- VPN

#### Properties

- [Documentation](https://dev.fingerprint.com/docs/smart-signals-overview)
- [OpenAPI](openapi/fingerprint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fingerprint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fingerprint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fingerprint Webhooks

Receive identification events at a configured HTTPS endpoint as they happen, carrying the same payload as the Events API for asynchronous server-side processing.

- **Human URL:** [https://dev.fingerprint.com/docs/webhooks](https://dev.fingerprint.com/docs/webhooks)
- **Base URL:** `https://api.fpjs.io`

#### Tags

- Webhooks
- Events
- Streaming

#### Properties

- [Documentation](https://dev.fingerprint.com/docs/webhooks)
- [OpenAPI](openapi/fingerprint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fingerprint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fingerprint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fingerprint Sealed Results

Decrypt sealed identification results delivered directly to the client and forwarded to your server, eliminating an extra Server API round-trip while keeping the full event payload server-validated.

- **Human URL:** [https://dev.fingerprint.com/docs/sealed-client-results](https://dev.fingerprint.com/docs/sealed-client-results)
- **Base URL:** `https://api.fpjs.io`

#### Tags

- Sealed Results
- Encryption
- Identification

#### Properties

- [Documentation](https://dev.fingerprint.com/docs/sealed-client-results)
- [OpenAPI](openapi/fingerprint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fingerprint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fingerprint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/fingerprintjs)
- [LinkedIn](https://www.linkedin.com/company/fingerprintjs)
- [Website](https://fingerprint.com)
- [Documentation](https://dev.fingerprint.com/docs)
- [Plans](plans/fingerprint-plans-pricing.yml)
- [Rate Limits](rate-limits/fingerprint-rate-limits.yml)
- [Fin Ops](finops/fingerprint-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
