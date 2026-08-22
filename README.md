# Portcast (portcast)

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
