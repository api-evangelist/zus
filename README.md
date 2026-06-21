# Zus Health (zus)

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
