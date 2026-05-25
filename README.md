# Routific (routific)

Routific is a Vancouver-based delivery management and route optimization software provider. Its platform combines smart route optimization, dispatch and live tracking, a driver mobile app, customer delivery notifications with real-time tracking, and proof of delivery. The standalone Route Optimization API exposes the same engine — solving Vehicle Routing Problems (VRP) and Pickup-and-Delivery Problems (PDP) — to SaaS integrators and channel partners. Routific has optimized over 191 million deliveries for more than 1,000 businesses since founding.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/routific/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- RouteOptimization, VRP, PickupAndDelivery, Logistics, LastMileDelivery, Delivery, FleetManagement, Dispatch, DeliveryManagement

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Routific Route Optimization API

Solves the Vehicle Routing Problem (VRP) and Pickup-and-Delivery Problem (PDP) for last-mile delivery fleets. Supports time-windows, capacity constraints, multi-depot fleets, driver shifts, balanced routes, traffic simulation, polyline output, toll avoidance, and Google or Here geocoding. Synchronous `/v1/vrp` handles small problems; asynchronous `/v1/vrp-long` and `/v1/pdp-long` process up to 2,500 visits per call via a `job_id` polling pattern. `/v1/fix` and `/v1/fix-pdp` insert new visits into existing solutions without re-solving.

**Base URL:** `https://api.routific.com`

**Authentication:** Bearer JWT — `Authorization: bearer <token>`

**Human URL:** [https://docs.routific.com/reference/getting-started](https://docs.routific.com/reference/getting-started)

#### Operations

| Method | Path | Operation |
|---|---|---|
| POST | `/v1/vrp` | Solve Vehicle Routing Problem (sync) |
| POST | `/v1/vrp-long` | Solve Vehicle Routing Problem (async; returns `job_id`) |
| POST | `/v1/pdp-long` | Solve Pickup-and-Delivery Problem (async) |
| GET  | `/jobs/{job_id}` | Get optimization job status / result |
| POST | `/v1/fix` | Insert new visits into existing VRP solution |
| POST | `/v1/fix-pdp` | Insert new visits into existing PDP solution |

#### Artifacts

- [OpenAPI](openapi/routific-route-optimization-api-openapi.yml)
- [JSON Schema — Visit](json-schema/routific-visit-schema.json)
- [JSON Schema — Vehicle](json-schema/routific-vehicle-schema.json)
- [JSON Schema — Solution](json-schema/routific-solution-schema.json)
- [JSON Schema — Job](json-schema/routific-job-schema.json)
- [JSON Structure — VRP Request](json-structure/routific-vrp-structure.json)
- [JSON-LD Context](json-ld/routific-context.jsonld)
- [Example — Synchronous VRP Solve](examples/routific-solve-vrp-example.json)
- [Example — Asynchronous VRP Solve](examples/routific-solve-vrp-long-example.json)
- [Example — Insert Visit Into Existing Solution](examples/routific-fix-vrp-example.json)
- [Spectral Ruleset](rules/routific-rules.yml)
- [Naftiko Capability — VRP](capabilities/route-optimization-vrp.yaml)
- [Naftiko Capability — PDP](capabilities/route-optimization-pdp.yaml)
- [Naftiko Capability — Jobs](capabilities/route-optimization-jobs.yaml)

#### Engine Options

`traffic`, `min_visits_per_vehicle`, `balance`, `visit_balance_coefficient`, `min_vehicles`, `shortest_distance`, `squash_durations`, `max_vehicle_overtime`, `max_visit_lateness`, `polylines`, `avoid_tolls`, `geocoder` (`google` or `here`).

#### Async Processing Times (`/vrp-long`)

| Visits | Average Time |
|---|---|
| < 100 | < 2s |
| 200 | 8s |
| 300 | 20s |
| 400 | 30s |
| 500 | 90s |
| 1,000 | ~4 min |
| 1,500 | ~8 min |
| 2,000 | ~18 min |
| 2,500 | ~22 min |

Hard limit: 2,500 visits per optimization call.

## SDKs

| Name | Language | Repo |
|---|---|---|
| routific | JavaScript / Node.js | [routific/routific-node-client](https://github.com/routific/routific-node-client) |
| routific | Ruby | [routific/routific-gem](https://github.com/routific/routific-gem) |

## Integrations

- Shopify
- WooCommerce
- Zapier

## Plans And Pricing

The Routific platform uses a per-order, volume-tiered pricing model (migrated from per-vehicle in mid-2024):

| Tier | Volume | Price |
|---|---|---|
| Free | Up to 100 orders/month | $0 |
| Paid (Flat) | 101–1,000 orders/month | $150 flat |
| Paid (Tiered) | 1,001–2,000 | $0.15 per additional order |
| Paid (Tiered) | 2,001–3,000 | $0.13 per additional order |
| Paid (Tiered) | 3,001–5,000 | $0.10 per additional order |
| Paid (Tiered) | 5,001–10,000 | $0.08 per additional order |
| Paid (Tiered) | 10,001–20,000 | $0.05 per additional order |
| Paid (Tiered) | 20,001–50,000 | $0.03 per additional order |
| Enterprise | 50,000+ | Contact sales |

The standalone Route Optimization API is licensed under custom volume terms — contact [support@routific.com](mailto:support@routific.com).

See [plans/routific-plans-pricing.yml](plans/routific-plans-pricing.yml), [rate-limits/routific-rate-limits.yml](rate-limits/routific-rate-limits.yml), and [finops/routific-finops.yml](finops/routific-finops.yml).

## Common

- [Portal](https://routific.com)
- [Developer Portal](https://dev.routific.com)
- [Developer Signup](https://dev.routific.com/signup)
- [API Documentation](https://docs.routific.com)
- [Quickstart](https://docs.routific.com/reference/getting-started)
- [Error Codes](https://docs.routific.com/reference/error-codes)
- [Routific Status](https://status.routific.com)
- [Help Center](https://help.routific.com)
- [Blog](https://routific.com/blog)
- [Pricing](https://routific.com/pricing)
- [GitHub Org](https://github.com/routific)
- [LinkedIn](https://www.linkedin.com/company/routific)
- [Twitter](https://twitter.com/routific)
- [Support Email](mailto:support@routific.com)

## Maintainer

- Kin Lane — [info@apievangelist.com](mailto:info@apievangelist.com) — [apievangelist.com](https://apievangelist.com)
