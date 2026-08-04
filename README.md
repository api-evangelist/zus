# Zus Health (zus)

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

Zus Health is a shared health-data platform that aggregates a patient's clinical history from external networks into the Zus Aggregated Profile (ZAP). It exposes a FHIR R4 (v4.0.1) REST API secured with OAuth2 Bearer tokens, Patient History APIs, document ingestion and retrieval, Zushooks webhooks, a GraphQL FHIR Query Service, and embeddable open-source React components.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/apis.yml)

## Tags

- Health
- FHIR
- Interoperability
- Patient Data
- Healthcare

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Zus Patients (FHIR)

Read, search, create, and update FHIR R4 Patient resources. The Patient.active field is the primary signal of an active treatment relationship and authorizes access to a patient's aggregated third-party data.

- **Human URL:** [https://docs.zushealth.com/docs/fhir-api](https://docs.zushealth.com/docs/fhir-api)
- **Base URL:** `https://api.zusapi.com/fhir`

#### Tags

- Patient
- FHIR
- Identity

#### Properties

- [Documentation](https://docs.zushealth.com/docs/fhir-api)
- [API Reference](https://docs.zushealth.com/reference/general)
- [OpenAPI](openapi/zus-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/zus.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zus.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Zus Aggregated Profile

The Zus Aggregated Profile (ZAP) assembles a longitudinal record from network partners. Patient History jobs retrieve external data into the FHIR Store, where it is deduplicated and summarized by Zus Lens.

- **Human URL:** [https://docs.zushealth.com/docs/accessing-the-zap](https://docs.zushealth.com/docs/accessing-the-zap)
- **Base URL:** `https://api.zusapi.com`

#### Tags

- ZAP
- Aggregation
- Patient History

#### Properties

- [Documentation](https://docs.zushealth.com/docs/accessing-the-zap)
- [Documentation](https://docs.zushealth.com/docs/zap-basics)
- [OpenAPI](openapi/zus-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/zus.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zus.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Zus FHIR Resources

Store and retrieve most FHIR R4 (v4.0.1) resource types - Observation, Condition, Encounter, MedicationStatement, Procedure, DiagnosticReport, and more - with read, search, create, update, patch, delete, and Bundle transactions.

- **Human URL:** [https://docs.zushealth.com/docs/fhir-rest-api-capabilities](https://docs.zushealth.com/docs/fhir-rest-api-capabilities)
- **Base URL:** `https://api.zusapi.com/fhir`

#### Tags

- FHIR
- Resources
- R4

#### Properties

- [Documentation](https://docs.zushealth.com/docs/fhir-rest-api-capabilities)
- [API Reference](https://docs.zushealth.com/reference/general)
- [OpenAPI](openapi/zus-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/zus.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zus.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Zus Document Retrieval

Ingest CDA and PDF documents and retrieve clinical documents through the FHIR DocumentReference and Binary resources, including base64-encoded payloads stored as submitted.

- **Human URL:** [https://docs.zushealth.com/docs/ingesting-documents](https://docs.zushealth.com/docs/ingesting-documents)
- **Base URL:** `https://api.zusapi.com/fhir`

#### Tags

- Documents
- DocumentReference
- Binary

#### Properties

- [Documentation](https://docs.zushealth.com/docs/ingesting-documents)
- [API Reference](https://docs.zushealth.com/reference/general)
- [OpenAPI](openapi/zus-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/zus.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zus.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Zus Subscriptions and Webhooks

Zushooks deliver inbound HTTPS callbacks when patient data is created or updated in the Zus FHIR Store - ADT events, medication pickups, lab results, and status changes - filtered by JQ criteria and authenticated with basic auth or OAuth client credentials.

- **Human URL:** [https://docs.zushealth.com/docs/zushooks](https://docs.zushealth.com/docs/zushooks)
- **Base URL:** `https://api.zusapi.com`

#### Tags

- Webhooks
- Subscriptions
- Zushooks

#### Properties

- [Documentation](https://docs.zushealth.com/docs/zushooks)
- [OpenAPI](openapi/zus-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/zus.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/zus.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/zushealth)
- [Website](https://zushealth.com)
- [Documentation](https://docs.zushealth.com)
- [Plans](plans/zus-plans-pricing.yml)
- [Rate Limits](rate-limits/zus-rate-limits.yml)
- [Fin Ops](finops/zus-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
