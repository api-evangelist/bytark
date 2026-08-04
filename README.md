# ByteArk (bytark)

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

ByteArk is a Thailand-based video streaming and content delivery platform founded in 2012 and headquartered in Bangkok. It provides video-on-demand (ByteArk Stream), live streaming (Fleet / Teatro), an S3-compatible object storage service, a global CDN, and a pre-configured web/mobile video player with DRM content protection. Developers integrate through REST APIs authenticated with personal access tokens and S3-compatible credentials.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/apis.yml)

## Tags

- Video
- Streaming
- Video on Demand
- Live Streaming
- CDN
- Object Storage
- Transcoding
- DRM
- Media

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### ByteArk Stream Video API

Create video records within a project, upload source files, list and filter the content library, and retrieve per-video information including the HLS primary playback URL. Uploads use the ByteArk Stream Video Upload SDK or direct form-data / resumable upload endpoints.

- **Human URL:** [https://docs.byteark.com/en/stream/](https://docs.byteark.com/en/stream/)
- **Base URL:** `https://stream.byteark.com/api/v1`

#### Tags

- Video
- Video on Demand
- Transcoding
- Media

#### Properties

- [Documentation](https://docs.byteark.com/en/stream/)
- [API Reference](https://docs.byteark.com/en/stream/developer-api-video-uploading.html)
- [OpenAPI](openapi/bytark-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bytark.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bytark.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ByteArk Live Streaming API

Fleet live transcode API to create, list, and delete live streaming channels. Returns an RTMP publish endpoint and stream key for ingest, an HLS (index.m3u8) viewing URL, and per-resolution transcode profiles. Also supports dropping a publisher and resetting the transcoder.

- **Human URL:** [https://docs.byteark.com/en/fleet-streaming/live-api-transcoder.html](https://docs.byteark.com/en/fleet-streaming/live-api-transcoder.html)
- **Base URL:** `https://fleet.byteark.com/api`

#### Tags

- Live Streaming
- Transcoding
- RTMP
- Media

#### Properties

- [Documentation](https://docs.byteark.com/en/fleet-streaming/live-api-transcoder.html)
- [API Reference](https://docs.byteark.com/en/fleet-streaming/live-api-transcoder.html)
- [OpenAPI](openapi/bytark-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bytark.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bytark.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ByteArk Storage API

S3-compatible object storage for storing and distributing files. Works with standard S3 SDKs and tooling (bucket and object operations - put, get, list, delete) using access-key / secret-key credentials. Tiered by redundancy (Basic, Standard, Extra Redundancy).

- **Human URL:** [https://docs.byteark.com/en/storage/](https://docs.byteark.com/en/storage/)
- **Base URL:** `https://storage.byteark.com`

#### Tags

- Object Storage
- S3
- Files
- Storage

#### Properties

- [Documentation](https://docs.byteark.com/en/storage/)
- [OpenAPI](openapi/bytark-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bytark.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bytark.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ByteArk CDN API

ByteArk Fleet CDN delivers web, app, and media assets across 15+ global points of presence with 10+ POPs in Thailand. Developer surfaces cover cache purge / invalidation and delivery configuration for origins served through the edge network.

- **Human URL:** [https://docs.byteark.com/en/fleet/](https://docs.byteark.com/en/fleet/)
- **Base URL:** `https://fleet.byteark.com/api`

#### Tags

- CDN
- Delivery
- Caching
- Edge

#### Properties

- [Documentation](https://docs.byteark.com/en/fleet/)
- [OpenAPI](openapi/bytark-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bytark.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bytark.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ByteArk Player API

Pre-configured HTML5 video player with framework packages for React, Vue, and Angular. Renders HLS playback with DRM content protection (including WisePlay), signed-URL access, and player-settings configuration surfaced through the Stream player settings.

- **Human URL:** [https://docs.byteark.com/en/stream/settings-video-players.html](https://docs.byteark.com/en/stream/settings-video-players.html)
- **Base URL:** `https://player.byteark.com`

#### Tags

- Player
- Embed
- Media
- DRM

#### Properties

- [Documentation](https://docs.byteark.com/en/stream/settings-video-players.html)
- [OpenAPI](openapi/bytark-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bytark.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bytark.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/byteark)
- [LinkedIn](https://www.linkedin.com/company/byteark)
- [Website](https://www.byteark.com/)
- [Documentation](https://docs.byteark.com/en/)
- [Plans](plans/bytark-plans-pricing.yml)
- [Rate Limits](rate-limits/bytark-rate-limits.yml)
- [Fin Ops](finops/bytark-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
