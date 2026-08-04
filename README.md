# X (Twitter) (twitter)

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

X (formerly Twitter) is a social media platform providing APIs for accessing and integrating with posts, users, spaces, direct messages, lists, media, trends, and real-time streaming data. The X API enables developers to build applications that read and write X data, manage advertising campaigns, and subscribe to real-time activity events. Available through pay-per-use credit-based pricing with enterprise options for high-volume access.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content

## Timestamps

- **Created:** 2025-07-29
- **Modified:** 2026-05-19

## APIs

### X API

The core X API providing programmatic access to posts, users, spaces, lists, direct messages, bookmarks, likes, reposts, follows, blocks, mutes, trends, communities, and compliance data. Supports post creation, search (recent and full-archive), timelines, filtered streams, sampled streams, and real-time data access. Uses OAuth 2.0 with PKCE or OAuth 1.0a authentication with credit-based pay-per-use pricing.

- **Human URL:** [https://docs.x.com/x-api](https://docs.x.com/x-api)
- **Base URL:** `https://api.x.com/2`

#### Tags

- Posts
- Users
- Spaces
- Lists
- Direct Messages
- Streaming
- Search
- Timelines

#### Properties

- [Documentation](https://docs.x.com/x-api)
- [Getting Started](https://docs.x.com/x-api/getting-started/make-your-first-request)
- [API Reference](https://docs.x.com/x-api)
- [Authentication](https://docs.x.com/resources/fundamentals/authentication)
- [Rate Limits](https://docs.x.com/x-api/fundamentals/rate-limits)
- [SDK](https://docs.x.com/sdks-and-tools/python-xdk)
- [SDK](https://docs.x.com/sdks-and-tools/typescript-xdk)
- [OpenAPI](openapi/x-api-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/x-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/x-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### X Ads API

The X Ads API enables programmatic management of advertising campaigns on the X platform including campaign creation and scheduling, custom audience building, creative management (draft posts, cards, media), and analytics retrieval for campaign performance metrics. Supports both synchronous and asynchronous analytics endpoints for reporting.

- **Human URL:** [https://docs.x.com/x-ads-api](https://docs.x.com/x-ads-api)
- **Base URL:** `https://ads-api.x.com`

#### Tags

- Advertising
- Campaigns
- Analytics
- Audiences
- Creatives

#### Properties

- [Documentation](https://docs.x.com/x-ads-api)
- [Getting Started](https://docs.x.com/x-ads-api/getting-started/create-a-campaign)
- [Rate Limits](https://docs.x.com/x-ads-api/fundamentals/rate-limiting)
- [Postman Collection](postman/x-ads-api-postman-collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Postman Collection](collections/x-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/x-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### X Activity API

The X Activity API provides real-time activity event subscriptions with sub-second delivery via streaming or webhooks. Subscribe to profile updates, follows, likes, reposts, and other user activity events. Recently exited beta and is now generally available.

- **Human URL:** [https://docs.x.com/x-activity-api](https://docs.x.com/x-activity-api)
- **Base URL:** `https://api.x.com`

#### Tags

- Activity
- Events
- Real-Time
- Streaming
- Webhooks

#### Properties

- [Documentation](https://docs.x.com/x-activity-api)
- [Postman Collection](collections/x-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/x-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [LinkedIn](https://www.linkedin.com/company/x-corp)
- [Portal](https://developer.x.com/en/portal/dashboard)
- [Getting Started](https://docs.x.com/x-api/getting-started/make-your-first-request)
- [Console](https://developer.x.com/en/portal/dashboard)
- [Sign Up](https://developer.x.com/en/portal/petition/essential/basic-info)
- [Authentication](https://docs.x.com/resources/fundamentals/authentication)
- [SDK](https://docs.x.com/sdks-and-tools/python-xdk)
- [SDK](https://docs.x.com/sdks-and-tools/typescript-xdk)
- [C L I](https://docs.x.com/sdks-and-tools/xurl)
- [Pricing](https://developer.x.com/en/portal/petition/essential/basic-info)
- [Terms of Service](https://developer.x.com/en/developer-terms/agreement-and-policy)
- [Privacy Policy](https://x.com/en/privacy)
- [Status Page](https://api.twitterstat.us/)
- [Support](https://devcommunity.x.com/)
- [Blog](https://blog.x.com/developer)
- [Release Notes](https://docs.x.com/changelog)
- [GitHub Organization](https://github.com/xdevplatform)
- [GitHub Repository](https://github.com/xdevplatform/xdk-python)
- [GitHub Repository](https://github.com/xdevplatform/xdk-typescript)
- [GitHub Repository](https://github.com/xdevplatform/xurl)
- [GitHub Repository](https://github.com/xdevplatform/xdk)
- [GitHub Repository](https://github.com/xdevplatform/twitter-api-java-sdk)
- [GitHub Repository](https://github.com/xdevplatform/twitter-ruby-ads-sdk)
- [Tools](https://github.com/xdevplatform/xmcp)
- [Sandbox](https://github.com/xdevplatform/playground)
- [Code Examples](https://github.com/xdevplatform/samples)
- [Code Examples](https://github.com/xdevplatform/xchat-bot-python)
- [Postman Workspace](https://docs.x.com/sdks-and-tools/postman)
- [Postman Collection](postman/x-api-v2-postman-collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [X (Twitter)](https://x.com/XDevelopers)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
