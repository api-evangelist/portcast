# Portcast (portcast)

Portcast is a predictive supply-chain visibility platform whose Container Tracking API delivers the full journey of an ocean container - milestones, vessel schedules, port codes, and machine-learning predicted ETAs and ETDs - in a single JSON response, tracked by container number, bill of lading, or booking number plus carrier SCAC, with push (webhook) callbacks on every update.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/apis.yml)

## Tags

- Supply Chain
- Container Tracking
- Logistics
- Predictive ETA
- Ocean Freight

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Portcast Container Tracking API

Upload an ocean shipment by container number, bill of lading, or booking number plus carrier SCAC and retrieve the full container journey - standardized milestone events, terminal details, transport plan, delays, and CO2 emissions - in one JSON response, with optional callback_url push updates.

- **Human URL:** [https://portcast.stoplight.io/docs/portcast-api/](https://portcast.stoplight.io/docs/portcast-api/)
- **Base URL:** `https://api.portcast.io/api/v2/eta`

#### Tags

- Container Tracking
- Ocean Freight
- Milestones

#### Properties

- [Documentation](https://portcast.stoplight.io/docs/portcast-api/5xrqljlsknrvm-input-data-guide)
- [API Reference](https://portcast.stoplight.io/docs/portcast-api/e120e68fcdc40-upload-using-container-number)
- [OpenAPI](openapi/portcast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/portcast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/portcast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Portcast Predictive ETA API

Machine-learning predicted ETA and ETD per leg surfaced through the tracking response sailing_info_tracking - predicted arrival and departure local times alongside scheduled and actual times, plus live AIS vessel position.

- **Human URL:** [https://www.portcast.io/predictive-visibility](https://www.portcast.io/predictive-visibility)
- **Base URL:** `https://api.portcast.io/api/v2/eta`

#### Tags

- Predictive ETA
- Machine Learning
- Ocean Freight

#### Properties

- [Documentation](https://portcast.stoplight.io/docs/portcast-api/7p466hav2ds7x-container-events-data-types)
- [OpenAPI](openapi/portcast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/portcast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/portcast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Portcast Vessel Schedules API

Vessel schedule, voyage, and live AIS position data surfaced through the tracking response - vessel name, IMO, MMSI, flag, inbound and outbound voyage numbers, and scheduled arrival and departure times at each port on the route.

- **Human URL:** [https://www.portcast.io/ocean-vessel-tracking-api](https://www.portcast.io/ocean-vessel-tracking-api)
- **Base URL:** `https://api.portcast.io/api/v2/eta`

#### Tags

- Vessel Schedules
- AIS
- Voyage

#### Properties

- [Documentation](https://www.portcast.io/ocean-vessel-tracking-api)
- [OpenAPI](openapi/portcast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/portcast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/portcast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Portcast Webhooks (Push API)

Register an HTTPS callback_url on a tracking upload and Portcast pushes the full tracking JSON object to your endpoint whenever container milestones or predictions are updated - eliminating polling.

- **Human URL:** [https://portcast.stoplight.io/docs/portcast-api/dxd93fedun52o-push-api](https://portcast.stoplight.io/docs/portcast-api/dxd93fedun52o-push-api)
- **Base URL:** `https://api.portcast.io/api/v2/eta`

#### Tags

- Webhooks
- Push
- Callbacks

#### Properties

- [Documentation](https://portcast.stoplight.io/docs/portcast-api/dxd93fedun52o-push-api)
- [OpenAPI](openapi/portcast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/portcast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/portcast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/portcast)
- [LinkedIn](https://www.linkedin.com/company/portcast)
- [Website](https://www.portcast.io/)
- [Documentation](https://portcast.stoplight.io/docs/portcast-api/)
- [Plans](plans/portcast-plans-pricing.yml)
- [Rate Limits](rate-limits/portcast-rate-limits.yml)
- [Fin Ops](finops/portcast-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
