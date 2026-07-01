# ByteArk (bytark)

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
