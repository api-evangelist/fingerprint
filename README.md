# Fingerprint (fingerprint)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
