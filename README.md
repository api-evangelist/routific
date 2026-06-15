# Routific (routific)

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
