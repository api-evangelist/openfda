# openFDA (openfda)

openFDA is the U.S. Food and Drug Administration's public data platform, providing Elasticsearch-backed REST APIs serving FDA-administered data on drugs, medical devices, foods, animal and veterinary products, and tobacco. Twenty-two endpoints under a single api.fda.gov base URL expose adverse event reports (FAERS, MAUDE, CAERS), recall enforcement reports, Structured Product Labeling, the National Drug Code Directory, Drugs@FDA approvals, drug shortages, device classification, 510(k) and PMA submissions, Unique Device Identifier records, registration and listing, NSDE drug data, FDA substance harmonization, and historical FDA documents. All endpoints share a Lucene-style search, sort, count, limit, and skip parameter surface, are released under CC0 Public Domain, and operate under a free api.data.gov key that lifts daily quotas to 120,000 requests.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Government
- Healthcare
- Drug
- Device
- Food
- Animal & Veterinary
- Tobacco
- Public Data
- Open Data
- Adverse Events
- Recalls
- Regulatory

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### openFDA Drug API

Drug-domain endpoints covering FAERS adverse event reports, Structured Product Labeling, drug recall enforcement reports, the National Drug Code Directory, Drugs@FDA approvals, and the FDA drug shortage database. Six Lucene-queryable endpoints under /drug/ that share a common search, sort, count, limit, and skip parameter surface.

- **Human URL:** [https://open.fda.gov/apis/drug/](https://open.fda.gov/apis/drug/)
- **Base URL:** `https://api.fda.gov`

#### Tags

- Drug
- Adverse Events
- Labeling
- Recalls
- NDC
- Government
- Healthcare

#### Properties

- [Documentation](https://open.fda.gov/apis/drug/)
- [API Reference](https://open.fda.gov/apis/drug/event/)
- [Documentation](https://open.fda.gov/apis/drug/label/)
- [Documentation](https://open.fda.gov/apis/drug/enforcement/)
- [Documentation](https://open.fda.gov/apis/drug/ndc/)
- [Documentation](https://open.fda.gov/apis/drug/drugsfda/)
- [Documentation](https://open.fda.gov/apis/drug/shortages/)
- [OpenAPI](openapi/openfda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openfda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openfda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### openFDA Device API

Device-domain endpoints covering MAUDE adverse event reports, device classification, 510(k) premarket notifications, PMA premarket approvals, UDI Unique Device Identifier records, device recall enforcement reports, device recalls, registration and listing, and the COVID-19 in vitro diagnostic serology test results dataset.

- **Human URL:** [https://open.fda.gov/apis/device/](https://open.fda.gov/apis/device/)
- **Base URL:** `https://api.fda.gov`

#### Tags

- Device
- Adverse Events
- 510(k)
- PMA
- UDI
- Recalls
- Classification
- Government
- Healthcare

#### Properties

- [Documentation](https://open.fda.gov/apis/device/)
- [Documentation](https://open.fda.gov/apis/device/event/)
- [Documentation](https://open.fda.gov/apis/device/classification/)
- [Documentation](https://open.fda.gov/apis/device/enforcement/)
- [Documentation](https://open.fda.gov/apis/device/recall/)
- [Documentation](https://open.fda.gov/apis/device/510k/)
- [Documentation](https://open.fda.gov/apis/device/pma/)
- [Documentation](https://open.fda.gov/apis/device/udi/)
- [Documentation](https://open.fda.gov/apis/device/registrationlisting/)
- [Documentation](https://open.fda.gov/apis/device/covid19serology/)
- [OpenAPI](openapi/openfda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openfda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openfda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### openFDA Food API

Food-domain endpoints covering food recall enforcement reports from the FDA Recall Enterprise System and CAERS food adverse event reports spontaneously submitted to FDA about foods and dietary supplements.

- **Human URL:** [https://open.fda.gov/apis/food/](https://open.fda.gov/apis/food/)
- **Base URL:** `https://api.fda.gov`

#### Tags

- Food
- Adverse Events
- Recalls
- Enforcement
- Government
- Healthcare

#### Properties

- [Documentation](https://open.fda.gov/apis/food/)
- [Documentation](https://open.fda.gov/apis/food/enforcement/)
- [Documentation](https://open.fda.gov/apis/food/event/)
- [OpenAPI](openapi/openfda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openfda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openfda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### openFDA Animal & Veterinary API

Animal & Veterinary endpoint serving adverse event reports involving animal drug and feed products, submitted voluntarily by veterinarians, drug manufacturers, and animal owners.

- **Human URL:** [https://open.fda.gov/apis/animalandveterinary/](https://open.fda.gov/apis/animalandveterinary/)
- **Base URL:** `https://api.fda.gov`

#### Tags

- Animal & Veterinary
- Adverse Events
- Government
- Healthcare

#### Properties

- [Documentation](https://open.fda.gov/apis/animalandveterinary/)
- [Documentation](https://open.fda.gov/apis/animalandveterinary/event/)
- [OpenAPI](openapi/openfda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openfda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openfda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### openFDA Tobacco API

Tobacco endpoint serving tobacco product problem reports submitted to the FDA Center for Tobacco Products, covering unexpected health or quality issues with regulated tobacco items.

- **Human URL:** [https://open.fda.gov/apis/tobacco/](https://open.fda.gov/apis/tobacco/)
- **Base URL:** `https://api.fda.gov`

#### Tags

- Tobacco
- Problem Reports
- Government
- Healthcare

#### Properties

- [Documentation](https://open.fda.gov/apis/tobacco/)
- [Documentation](https://open.fda.gov/apis/tobacco/problem/)
- [OpenAPI](openapi/openfda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openfda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openfda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### openFDA Other API

Cross-cutting reference datasets including the NDC SPL Data Elements file of all drug products marketed in the US, the FDA Substance Registration System harmonized substance data, and historical FDA documents and enforcement actions.

- **Human URL:** [https://open.fda.gov/apis/other/](https://open.fda.gov/apis/other/)
- **Base URL:** `https://api.fda.gov`

#### Tags

- NSDE
- Substance
- Historical Documents
- Government
- Healthcare

#### Properties

- [Documentation](https://open.fda.gov/apis/other/)
- [Documentation](https://open.fda.gov/apis/other/nsde/)
- [Documentation](https://open.fda.gov/apis/other/substance/)
- [Documentation](https://open.fda.gov/apis/other/historicaldocument/)
- [OpenAPI](openapi/openfda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openfda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openfda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://open.fda.gov/)
- [Documentation](https://open.fda.gov/apis/)
- [Authentication](https://open.fda.gov/apis/authentication/)
- [Sign Up](https://api.data.gov/signup/)
- [Getting Started](https://open.fda.gov/apis/try-the-api/)
- [API Reference](https://open.fda.gov/apis/query-parameters/)
- [API Reference](https://open.fda.gov/apis/query-syntax/)
- [API Reference](https://open.fda.gov/apis/advanced-syntax/)
- [Errors](https://open.fda.gov/apis/errors/)
- [Documentation](https://open.fda.gov/apis/downloads/)
- [Status Page](https://open.fda.gov/about/status/)
- [Changelog](https://open.fda.gov/updates/)
- [Forum](https://open.fda.gov/community/)
- [GitHub Organization](https://github.com/FDA)
- [GitHub Repository](https://github.com/FDA/openfda)
- [GitHub Repository](https://github.com/FDA/open.fda.gov)
- [Documentation](https://www.fda.gov/)
- [Support](https://www.fda.gov/about-fda/contact-fda)
- [License](https://creativecommons.org/publicdomain/zero/1.0/)
- [Terms of Service](https://open.fda.gov/terms/)
- [Privacy Policy](https://www.fda.gov/about-website/website-policies)
- [Rules](rules/openfda-rules.yml)
- [Spectral Rules](rules/openfda-rules.yml)
- [J S O N- L D](json-ld/openfda-context.jsonld)
- [Vocabulary](vocabulary/openfda-vocabulary.yml)
- [Rate Limits](rate-limits/openfda-rate-limits.yml)
- [JSON Schema](json-schema/openfda-search-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/openfda-drug-event-example.json)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
