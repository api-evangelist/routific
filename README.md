# Routific (routific)

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

Routific is a Vancouver-based delivery management and route optimization software provider. Its platform combines smart route optimization, dispatch and live tracking, a driver mobile app, customer delivery notifications with real-time tracking, and proof of delivery. The standalone Route Optimization API exposes the same engine — solving Vehicle Routing Problems (VRP) and Pickup-and-Delivery Problems (PDP) — to SaaS integrators and channel partners. Routific has optimized over 191 million deliveries for more than 1,000 businesses since founding.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- RouteOptimization
- VRP
- PickupAndDelivery
- Logistics
- LastMileDelivery
- Delivery
- FleetManagement
- Dispatch
- DeliveryManagement

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Routific Route Optimization API

Routific's Route Optimization API solves the Vehicle Routing Problem (VRP) and Pickup-and-Delivery Problem (PDP) for last-mile delivery fleets. It supports time-windows, capacity constraints, multi-depot fleets, driver shifts, balanced routes, traffic simulation, polyline output, toll avoidance, and Google or Here geocoding. Synchronous /v1/vrp handles small problems; asynchronous /v1/vrp-long and /v1/pdp-long process up to 2,500 visits per call via a job_id polling pattern. /v1/fix and /v1/fix-pdp insert new visits into existing solutions without re-solving.

- **Human URL:** [https://docs.routific.com/reference/getting-started](https://docs.routific.com/reference/getting-started)
- **Base URL:** `https://api.routific.com`

#### Tags

- RouteOptimization
- VRP
- PickupAndDelivery
- Logistics
- Delivery
- FleetManagement

#### Properties

- [Documentation](https://docs.routific.com/reference/getting-started)
- [Documentation](https://docs.routific.com/reference/options)
- [Documentation](https://docs.routific.com/reference/re-optimize-solution)
- [Documentation](https://docs.routific.com/reference/error-codes)
- [L L Ms Txt](https://docs.routific.com/llms.txt)
- [OpenAPI](openapi/routific-route-optimization-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/routific-route-optimization-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/routific-route-optimization-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/routific-visit-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/routific-vehicle-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/routific-solution-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/routific-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/routific-vrp-structure.json)
- [JSON-LD](json-ld/routific-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/routific-solve-vrp-example.json)
- [Example](examples/routific-solve-vrp-long-example.json)
- [Example](examples/routific-fix-vrp-example.json)
- [Spectral Rules](rules/routific-rules.yml)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/routific)
- [Twitter](https://twitter.com/routific)
- [Git Hub](https://github.com/routific)
- [Portal](https://routific.com)
- [Developer](https://dev.routific.com)
- [Signup](https://dev.routific.com/signup)
- [Documentation](https://docs.routific.com)
- [Documentation](https://docs.routific.com/reference/getting-started)
- [Errors](https://docs.routific.com/reference/error-codes)
- [Status Page](https://status.routific.com)
- [Support](https://help.routific.com)
- [Blog](https://routific.com/blog)
- [Pricing](https://routific.com/pricing)
- [Documentation](https://academy.routific.com)
- [Support](mailto:support@routific.com)
- [Plans](plans/routific-plans-pricing.yml)
- [Rate Limits](rate-limits/routific-rate-limits.yml)
- [Fin Ops](finops/routific-finops.yml)
- [Vocabulary](vocabulary/routific-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
