# X (Twitter) (twitter)
X (formerly Twitter) is a social media platform providing APIs for accessing and integrating with posts, users, spaces, direct messages, lists, media, trends, and real-time streaming data. The X API enables developers to build applications that read and write X data, manage advertising campaigns, and subscribe to real-time activity events.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Social Media, Microblogging, Real-Time Data, Streaming, Advertising, Content

## Timestamps

- **Created:** 2025-07-29
- **Modified:** 2026-04-17

## APIs

### X API
The core X API providing programmatic access to posts, users, spaces, lists, direct messages, bookmarks, likes, reposts, follows, blocks, mutes, trends, communities, and compliance data. Supports post creation, search (recent and full-archive), timelines, filtered streams, sampled streams, and real-time data access.

**Human URL:** [https://docs.x.com/x-api](https://docs.x.com/x-api)

#### Tags:

 - Posts, Users, Spaces, Lists, Direct Messages, Streaming, Search, Timelines

#### Properties

- [Documentation](https://docs.x.com/x-api)
- [Getting Started](https://docs.x.com/x-api/getting-started/make-your-first-request)
- [API Reference](https://docs.x.com/x-api)
- [Authentication](https://docs.x.com/resources/fundamentals/authentication)
- [Rate Limits](https://docs.x.com/x-api/fundamentals/rate-limits)
- [Python XDK](https://docs.x.com/sdks-and-tools/python-xdk)
- [TypeScript XDK](https://docs.x.com/sdks-and-tools/typescript-xdk)

### X Ads API
The X Ads API enables programmatic management of advertising campaigns on the X platform including campaign creation and scheduling, custom audience building, creative management, and analytics retrieval for campaign performance metrics.

**Human URL:** [https://docs.x.com/x-ads-api](https://docs.x.com/x-ads-api)

#### Tags:

 - Advertising, Campaigns, Analytics, Audiences, Creatives

#### Properties

- [Documentation](https://docs.x.com/x-ads-api)
- [Getting Started](https://docs.x.com/x-ads-api/getting-started/create-a-campaign)
- [Rate Limits](https://docs.x.com/x-ads-api/fundamentals/rate-limiting)

### X Activity API
The X Activity API provides real-time activity event subscriptions with sub-second delivery via streaming or webhooks. Subscribe to profile updates, follows, likes, reposts, and other user activity events.

**Human URL:** [https://docs.x.com/x-activity-api](https://docs.x.com/x-activity-api)

#### Tags:

 - Activity, Events, Real-Time, Streaming, Webhooks

#### Properties

- [Documentation](https://docs.x.com/x-activity-api)

## Common Properties

- [Portal](https://developer.x.com/en/portal/dashboard)
- [Getting Started](https://docs.x.com/x-api/getting-started/make-your-first-request)
- [Console](https://developer.x.com/en/portal/dashboard)
- [Sign Up](https://developer.x.com/en/portal/petition/essential/basic-info)
- [Authentication](https://docs.x.com/resources/fundamentals/authentication)
- [Python XDK](https://docs.x.com/sdks-and-tools/python-xdk)
- [TypeScript XDK](https://docs.x.com/sdks-and-tools/typescript-xdk)
- [xurl CLI](https://docs.x.com/sdks-and-tools/xurl)
- [Pricing](https://developer.x.com/en/portal/petition/essential/basic-info)
- [Terms of Service](https://developer.x.com/en/developer-terms/agreement-and-policy)
- [Privacy Policy](https://x.com/en/privacy)
- [Status Page](https://api.twitterstat.us/)
- [Support](https://devcommunity.x.com/)
- [Blog](https://blog.x.com/developer)
- [Release Notes](https://docs.x.com/changelog)
- [GitHub Organization](https://github.com/xdevplatform)
- [Python XDK Repo](https://github.com/xdevplatform/xdk-python)
- [TypeScript XDK Repo](https://github.com/xdevplatform/xdk-typescript)
- [xurl CLI Repo](https://github.com/xdevplatform/xurl)
- [XDK Generator](https://github.com/xdevplatform/xdk)
- [Java SDK](https://github.com/xdevplatform/twitter-api-java-sdk)
- [Ruby Ads SDK](https://github.com/xdevplatform/twitter-ruby-ads-sdk)
- [MCP Server](https://github.com/xdevplatform/xmcp)
- [API Playground](https://github.com/xdevplatform/playground)
- [Code Samples](https://github.com/xdevplatform/samples)
- [Chat Bot Example](https://github.com/xdevplatform/xchat-bot-python)
- [Postman](https://docs.x.com/sdks-and-tools/postman)
- [X](https://x.com/XDevelopers)

## Features

| Name | Description |
|------|-------------|
| Post Management | Create, delete, edit, repost, quote, like, and bookmark posts programmatically. |
| Real-Time Streaming | Access filtered streams, sampled streams, firehose, and language-specific streams for real-time post data. |
| Full-Archive Search | Search the complete archive of public posts with advanced query operators and date filtering. |
| User Lookup and Management | Look up users by ID or username, manage follows, blocks, mutes, and retrieve user metrics. |
| Spaces | Discover and look up live audio Spaces with host, speaker, and listener data. |
| Direct Messages | Send and receive direct messages, create conversations, and manage participants. |
| Lists | Create, manage, and query lists including membership, followers, and pinned lists. |
| Trends | Access personalized and geographic trending topics. |
| Media Upload | Upload images, videos, and large files using chunked upload with metadata and subtitle support. |
| Compliance | Access compliance streams and batch jobs for data deletion and user protection events. |
| Communities and Community Notes | Access community data and community notes for collaborative fact-checking. |
| Ad Campaign Management | Programmatically create, schedule, and manage advertising campaigns with targeting and budget controls. |

## Use Cases

| Name | Description |
|------|-------------|
| Social Listening | Monitor brand mentions, sentiment, and conversations in real-time using filtered streams and search endpoints. |
| Content Publishing | Automate post creation, scheduling, and thread publishing for social media management platforms. |
| Analytics and Reporting | Retrieve post metrics, user engagement data, and campaign performance for business intelligence. |
| Bot Development | Build automated accounts that respond to mentions, post updates, or provide customer service. |
| Research and Academic Analysis | Access full-archive search and streaming data for social media research and trend analysis. |
| Advertising Automation | Programmatically manage ad campaigns, audiences, creatives, and bidding strategies at scale. |
| Real-Time Event Monitoring | Track live events, breaking news, and trending topics with streaming APIs and trend endpoints. |
| Community Management | Manage followers, lists, and direct messages for community engagement and moderation. |

## Integrations

| Name | Description |
|------|-------------|
| Postman | Official Postman collections for exploring and testing X API endpoints interactively. |
| MCP Servers | Integration with AI tools and agents through Model Context Protocol servers. |
| Webhook Delivery | Real-time event delivery via webhooks for the Activity API. |

## Solutions

| Name | Description |
|------|-------------|
| X API Pay-Per-Use | Credit-based pricing with no commitments. Pay only for what you use with access to core X API endpoints. |
| X API Enterprise | High-volume access with custom rate limits, dedicated account management, full firehose, and premium support. |
| X Ads API | Advertising platform API for campaign management, audience targeting, creative management, and analytics. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [X API v2](openapi/x-api-openapi.json) — 139 endpoints, 440 schemas (official, version 2.161)

### Postman

- [X API v2 Postman Collection](postman/x-api-v2-postman-collection.json)
- [X Ads API Postman Collection](postman/x-ads-api-postman-collection.json)

### JSON Schema

26 standalone JSON Schema files extracted from the X API v2 OpenAPI spec in [json-schema/](json-schema/).

### JSON Structure

26 JSON Structure files converted from JSON Schema in [json-structure/](json-structure/).

### JSON-LD

- [X API Context](json-ld/x-api-context.jsonld) — 23 types, 118 properties with schema.org alignments

### Examples

26 realistic example JSON files generated from JSON Schema in [examples/](examples/).

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Posts](capabilities/shared/posts.yaml) — 17 operations for post management, search, timelines, and analytics
- [Users](capabilities/shared/users.yaml) — 14 operations for user lookup, follows, blocks, and mutes
- [Streaming](capabilities/shared/streaming.yaml) — 12 operations for firehose, filtered, sampled, and compliance streams
- [Direct Messages](capabilities/shared/direct-messages.yaml) — 9 operations for conversations and message management
- [Lists](capabilities/shared/lists.yaml) — 17 operations for list CRUD, membership, and following
- [Spaces](capabilities/shared/spaces.yaml) — 6 operations for audio space discovery and lookup
- [Media](capabilities/shared/media.yaml) — 10 operations for chunked upload, metadata, and subtitles
- [Bookmarks](capabilities/shared/bookmarks.yaml) — 5 operations for bookmark management and folders

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Content Publishing](capabilities/content-publishing.yaml) | Posts + Media + Bookmarks + Lists | 20 | Social Media Manager / Content Creator |
| [Social Listening](capabilities/social-listening.yaml) | Posts + Streaming + Users | 18 | Data Analyst / Brand Manager / Researcher |
| [Engagement](capabilities/engagement.yaml) | Users + Direct Messages + Spaces | 16 | Community Manager / Customer Support |
| [Compliance and Data](capabilities/compliance-and-data.yaml) | Streaming + Posts | 7 | Compliance Officer / Data Engineer |

## Vocabulary

- [X (Twitter) Vocabulary](vocabulary/twitter-vocabulary.yaml) — Unified taxonomy mapping 20 resources, 17 actions, 4 workflows, and 11 personas across operational (3 APIs, 163 operations) and capability (8 shared definitions) dimensions

## Rules

- [Twitter Spectral Rules](rules/twitter-spectral-rules.yml) — 53 rules across 12 categories enforcing X API conventions including snake_case paths, camelCase operationIds, field selection parameters, and data wrapper patterns

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
