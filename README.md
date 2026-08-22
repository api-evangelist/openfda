# openFDA (openfda)

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
