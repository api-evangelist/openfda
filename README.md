# openFDA (openfda)

openFDA is the U.S. Food and Drug Administration's public data platform, providing Elasticsearch-backed REST APIs serving FDA-administered data on drugs, medical devices, foods, animal and veterinary products, and tobacco. Twenty-two endpoints under a single `api.fda.gov` base URL expose adverse event reports (FAERS, MAUDE, CAERS), recall enforcement reports, Structured Product Labeling, the National Drug Code Directory, Drugs@FDA approvals, drug shortages, device classification, 510(k) and PMA submissions, Unique Device Identifier records, registration and listing, NSDE drug data, FDA substance harmonization, and historical FDA documents. All endpoints share a Lucene-style `search`, `sort`, `count`, `limit`, and `skip` parameter surface, are released under CC0 Public Domain, and operate under a free api.data.gov key that lifts daily quotas to 120,000 requests.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=government-api-evangelist&utm_content=repo)

## Tags

 - Government, Healthcare, Drug, Device, Food, Animal & Veterinary, Tobacco, Public Data, Open Data, Adverse Events, Recalls, Regulatory

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Rate Limits

| Tier | Auth | Per Minute | Per Day | Scope |
|---|---|---|---|---|
| Anonymous | none | 240 | 1,000 | per IP address |
| Registered | `api_key` (query or HTTP Basic password) | 240 | 120,000 | per API key |

Pagination is capped at `skip=25,000` with `limit=1,000` per request. Use the [bulk downloads](https://open.fda.gov/apis/downloads/) for deeper traversal. See [`rate-limits/openfda-rate-limits.yml`](rate-limits/openfda-rate-limits.yml).

## APIs

### openFDA Drug API
Drug-domain endpoints covering FAERS adverse events, Structured Product Labeling, drug recall enforcement reports, the National Drug Code Directory, Drugs@FDA approvals, and the FDA drug shortage database.

**Human URL:** [https://open.fda.gov/apis/drug/](https://open.fda.gov/apis/drug/)
**Base URL:** `https://api.fda.gov`

- [Documentation — Drug](https://open.fda.gov/apis/drug/)
- [Documentation — Adverse Events (FAERS)](https://open.fda.gov/apis/drug/event/)
- [Documentation — Labeling (SPL)](https://open.fda.gov/apis/drug/label/)
- [Documentation — Recall Enforcement](https://open.fda.gov/apis/drug/enforcement/)
- [Documentation — NDC Directory](https://open.fda.gov/apis/drug/ndc/)
- [Documentation — Drugs@FDA](https://open.fda.gov/apis/drug/drugsfda/)
- [Documentation — Drug Shortages](https://open.fda.gov/apis/drug/shortages/)
- [OpenAPI](openapi/openfda-openapi.yml)
- [Naftiko Capability](capabilities/openfda-drug.yaml)

### openFDA Device API
Device-domain endpoints covering MAUDE adverse events, device classification, 510(k) premarket notifications, PMA premarket approvals, UDI records, device recall enforcement, device recalls, registration and listing, and the COVID-19 in vitro diagnostic serology dataset.

**Human URL:** [https://open.fda.gov/apis/device/](https://open.fda.gov/apis/device/)
**Base URL:** `https://api.fda.gov`

- [Documentation — Device](https://open.fda.gov/apis/device/)
- [Documentation — Adverse Events (MAUDE)](https://open.fda.gov/apis/device/event/)
- [Documentation — Classification](https://open.fda.gov/apis/device/classification/)
- [Documentation — Recall Enforcement](https://open.fda.gov/apis/device/enforcement/)
- [Documentation — Recalls](https://open.fda.gov/apis/device/recall/)
- [Documentation — 510(k)](https://open.fda.gov/apis/device/510k/)
- [Documentation — PMA](https://open.fda.gov/apis/device/pma/)
- [Documentation — UDI](https://open.fda.gov/apis/device/udi/)
- [Documentation — Registration and Listing](https://open.fda.gov/apis/device/registrationlisting/)
- [Documentation — COVID-19 Serology](https://open.fda.gov/apis/device/covid19serology/)
- [OpenAPI](openapi/openfda-openapi.yml)
- [Naftiko Capability](capabilities/openfda-device.yaml)

### openFDA Food API
Food-domain endpoints covering food recall enforcement reports from the FDA Recall Enterprise System and CAERS food adverse event reports for foods and dietary supplements.

**Human URL:** [https://open.fda.gov/apis/food/](https://open.fda.gov/apis/food/)
**Base URL:** `https://api.fda.gov`

- [Documentation — Food](https://open.fda.gov/apis/food/)
- [Documentation — Recall Enforcement](https://open.fda.gov/apis/food/enforcement/)
- [Documentation — Adverse Events (CAERS)](https://open.fda.gov/apis/food/event/)
- [OpenAPI](openapi/openfda-openapi.yml)
- [Naftiko Capability](capabilities/openfda-food.yaml)

### openFDA Animal & Veterinary API
Adverse event reports involving animal drug and feed products, submitted voluntarily by veterinarians, drug manufacturers, and animal owners.

**Human URL:** [https://open.fda.gov/apis/animalandveterinary/](https://open.fda.gov/apis/animalandveterinary/)
**Base URL:** `https://api.fda.gov`

- [Documentation — Animal & Veterinary](https://open.fda.gov/apis/animalandveterinary/)
- [Documentation — Adverse Events](https://open.fda.gov/apis/animalandveterinary/event/)
- [OpenAPI](openapi/openfda-openapi.yml)
- [Naftiko Capability](capabilities/openfda-animal-veterinary.yaml)

### openFDA Tobacco API
Tobacco product problem reports submitted to the FDA Center for Tobacco Products covering unexpected health or quality issues with regulated tobacco items.

**Human URL:** [https://open.fda.gov/apis/tobacco/](https://open.fda.gov/apis/tobacco/)
**Base URL:** `https://api.fda.gov`

- [Documentation — Tobacco](https://open.fda.gov/apis/tobacco/)
- [Documentation — Problem Reports](https://open.fda.gov/apis/tobacco/problem/)
- [OpenAPI](openapi/openfda-openapi.yml)
- [Naftiko Capability](capabilities/openfda-tobacco.yaml)

### openFDA Other API
Cross-cutting reference datasets including the NDC SPL Data Elements file (NSDE) of all drug products marketed in the US, the FDA Substance Registration System harmonized substance data, and historical FDA documents and enforcement actions.

**Human URL:** [https://open.fda.gov/apis/other/](https://open.fda.gov/apis/other/)
**Base URL:** `https://api.fda.gov`

- [Documentation — Other](https://open.fda.gov/apis/other/)
- [Documentation — NSDE](https://open.fda.gov/apis/other/nsde/)
- [Documentation — Substance](https://open.fda.gov/apis/other/substance/)
- [Documentation — Historical Documents](https://open.fda.gov/apis/other/historicaldocument/)
- [OpenAPI](openapi/openfda-openapi.yml)
- [Naftiko Capability](capabilities/openfda-other.yaml)

## Common Resources

- [openFDA Portal](https://open.fda.gov/)
- [API Endpoints](https://open.fda.gov/apis/)
- [Authentication & API Keys](https://open.fda.gov/apis/authentication/)
- [api.data.gov Signup](https://api.data.gov/signup/)
- [Try the API](https://open.fda.gov/apis/try-the-api/)
- [Query Parameters Reference](https://open.fda.gov/apis/query-parameters/)
- [Query Syntax (Lucene)](https://open.fda.gov/apis/query-syntax/)
- [Advanced Query Syntax](https://open.fda.gov/apis/advanced-syntax/)
- [Error Reference](https://open.fda.gov/apis/errors/)
- [Bulk Downloads](https://open.fda.gov/apis/downloads/)
- [openFDA Status](https://open.fda.gov/about/status/)
- [openFDA Updates / Changelog](https://open.fda.gov/updates/)
- [Community](https://open.fda.gov/community/)
- [FDA GitHub Organization](https://github.com/FDA)
- [openFDA on GitHub](https://github.com/FDA/openfda)
- [open.fda.gov web app](https://github.com/FDA/open.fda.gov)
- [U.S. Food and Drug Administration](https://www.fda.gov/)
- [Contact FDA](https://www.fda.gov/about-fda/contact-fda)
- [License — CC0 1.0 Universal Public Domain](https://creativecommons.org/publicdomain/zero/1.0/)
- [openFDA Terms of Service](https://open.fda.gov/terms/)
- [FDA Privacy Policy](https://www.fda.gov/about-website/website-policies)

## Generated Artifacts

| Artifact | Path |
|---|---|
| OpenAPI 3.0 spec (22 operations across 6 domains) | [`openapi/openfda-openapi.yml`](openapi/openfda-openapi.yml) |
| Usage rules (Spectral-compatible) | [`rules/openfda-rules.yml`](rules/openfda-rules.yml) |
| Naftiko capability — Drug | [`capabilities/openfda-drug.yaml`](capabilities/openfda-drug.yaml) |
| Naftiko capability — Device | [`capabilities/openfda-device.yaml`](capabilities/openfda-device.yaml) |
| Naftiko capability — Food | [`capabilities/openfda-food.yaml`](capabilities/openfda-food.yaml) |
| Naftiko capability — Animal & Veterinary | [`capabilities/openfda-animal-veterinary.yaml`](capabilities/openfda-animal-veterinary.yaml) |
| Naftiko capability — Tobacco | [`capabilities/openfda-tobacco.yaml`](capabilities/openfda-tobacco.yaml) |
| Naftiko capability — Other | [`capabilities/openfda-other.yaml`](capabilities/openfda-other.yaml) |
| Rate-limits (API Commons 0.1) | [`rate-limits/openfda-rate-limits.yml`](rate-limits/openfda-rate-limits.yml) |
| JSON-LD context | [`json-ld/openfda-context.jsonld`](json-ld/openfda-context.jsonld) |
| Domain vocabulary | [`vocabulary/openfda-vocabulary.yml`](vocabulary/openfda-vocabulary.yml) |

## Features

- Six product-domain APIs (drug, device, food, animal & veterinary, tobacco, other) under a single `api.fda.gov` base URL
- Twenty-two Lucene-queryable JSON endpoints sharing `search`, `sort`, `count`, `limit`, and `skip` parameters
- Aggregation via the `count` parameter returns frequency histograms on any field without retrieving documents
- Bulk download of every dataset as JSON archives partitioned for resumable transfer
- Optional free api.data.gov API key lifts the per-IP daily quota from 1,000 to 120,000 requests
- Per-minute ceiling of 240 requests/min applies uniformly to anonymous and keyed callers
- Pagination capped at `skip=25,000` with `limit=1,000`; deeper traversal requires bulk downloads
- All endpoints are CC0 Public Domain — no attribution required for commercial or research reuse
- Harmonized `openfda` block on most documents links each record back to NDC, UNII, SPL Set ID, and other identifiers
- HTTPS-only with HTTP Basic or query-parameter key authentication
- Public status page and email list for outage and breaking-change notifications
- Active developer community via the openFDA GitHub organization and community forum

## Use Cases

- **Adverse Event Surveillance** — Mine FAERS, MAUDE, CAERS, and animal/veterinary reports for safety signals across product domains.
- **Recall Monitoring** — Subscribe to drug, device, and food recall enforcement reports for clinical, retail, or supply-chain dashboards.
- **Drug Labeling Apps** — Embed authoritative SPL indications, dosage, warnings, and ingredient sections into consumer or clinical applications.
- **Regulatory Intelligence** — Track 510(k) clearances, PMA approvals, and Drugs@FDA submissions to monitor competitor and pipeline activity.
- **Identifier Resolution** — Look up NDC, UDI, UNII, and SPL Set IDs across product domains for claims, EHR, and supply-chain integrations.
- **Public-Health Research** — CC0-licensed adverse outcome, recall, and enforcement data for academic and journalistic investigation.
- **Supply-Chain Risk** — Cross-reference drug shortage status, recall actions, and registration listings to detect upstream supply disruptions.

## Integrations

- **api.data.gov** — Federal API gateway issuing and enforcing the openFDA API key.
- **data.gov** — Federal open-data portal cataloging openFDA datasets as DCAT-compliant resources.
- **NIH RxNorm** — Common join target for NDC and Drugs@FDA records.
- **NLM DailyMed** — Authoritative SPL drug labeling repository mirrored by openFDA.
- **GUDID (Global UDI Database)** — Source of openFDA device UDI records.
- **FAERS Public Dashboard** — Same FAERS data exposed by openFDA's drug adverse event endpoint.

## Solutions

- **Pharmacovigilance** — Continuously ingest drug, device, and food adverse events for safety signal detection.
- **Recall and Withdrawal Alerting** — Power weekly recall enforcement notification workflows across drug, device, and food domains.
- **Regulatory Filings Intelligence** — Aggregate 510(k), PMA, and Drugs@FDA submissions for competitive analysis.
- **Clinical Decision Support References** — Surface FDA labeling content as a reference layer (explicitly not for clinical decision-making per openFDA terms).

## Important Notice

openFDA is **not** for clinical use, public health alerting, or product-level safety decisions. The data is unvalidated, non-causal, and FDA does not update recall status after classification. See [`rules/openfda-rules.yml`](rules/openfda-rules.yml) for the full operational and compliance ruleset.

## Maintainers

- **Kin Lane** ([apievangelist.com](https://apievangelist.com)) — [@apievangelist](https://x.com/apievangelist) — info@apievangelist.com

---

*This profile is part of the [API Evangelist](https://apievangelist.com) network. APIs.json specification version `0.16`.*
