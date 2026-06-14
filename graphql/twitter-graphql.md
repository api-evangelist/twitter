# Twitter (X) GraphQL Schema

## Overview

This conceptual GraphQL schema models the Twitter (X) API v2 data model. The X API v2 is a REST API available at `https://api.x.com/2`, but the types defined here represent the full surface of objects, relationships, and operations exposed by that API. This schema captures tweets, users, spaces, lists, direct messages, media, polls, streams, compliance, and advertising data.

## Source

- API Provider: X (Twitter)
- API Version: X API v2
- Base URL: `https://api.x.com/2`
- Documentation: https://docs.x.com/x-api
- GitHub Organization: https://github.com/xdevplatform

## Schema Source

Conceptual — derived from the X API v2 REST documentation, OpenAPI specification, and official SDK definitions. Not a native GraphQL endpoint.

## Authentication

X API v2 uses OAuth 2.0 with PKCE (recommended) or OAuth 1.0a. App-only auth uses Bearer tokens. User context operations require user-delegated tokens.

## Types Summary

| Category | Types |
|---|---|
| Tweet | Tweet, TweetAttachment, TweetMention, TweetAnnotation, TweetContextAnnotation, TweetEntity, TweetEntityUrl, TweetEntityHashtag, TweetEntityCashtag, TweetEntityMention, TweetExpansions, TweetMetrics, TweetOrganicMetrics, TweetNonPublicMetrics, TweetPublicMetrics, TweetData, TweetEditControls, TweetGeo, TweetReferencedTweet, TweetWithheld |
| User | User, UserEntities, UserMentions, UserDescription, UserUrl, UserVerified, UserProtected, UserMetrics, UserData, UserWithheld, UserPublicMetrics |
| Space | Space, SpaceTopic, SpaceParticipant, SpaceInvitedUser |
| List | List, ListMember |
| Media | Media, Video, Gif, Photo, MediaVariant, MediaMetrics, MediaNonPublicMetrics, MediaOrganicMetrics, MediaPromotedMetrics |
| Poll | Poll, PollOption |
| Direct Message | DirectMessage, DMConversation, DMParticipant, DMEvent, DMAttachment |
| Stream | StreamRule, FilterRule, StreamRuleTag |
| Search & Timelines | SearchResult, TimelinesResult, SearchMeta |
| Place & Geo | Place, PlaceGeo, Coordinates |
| Compliance | ComplianceEvent, ComplianceJob, ComplianceJobResult |
| Context | ContextAnnotationDomain, ContextAnnotationEntity |
| Usage | UsageTweet, UsageData |
| Expansion | Expansion |
| Auth | AccessToken, ApiKey, OAuthToken |
| Error | Error, Problem, ResourceNotFoundProblem, AuthorizationProblem, GenericProblem |
| Pagination | Meta, PaginationMeta |
| Misc | Trend, Community, CommunityRule, CommunityMember |

## Query Operations

- `tweet(id: ID!)` — Look up a single tweet by ID
- `tweets(ids: [ID!]!)` — Look up multiple tweets by ID
- `searchRecent(query: String!, ...)` — Search recent tweets (last 7 days)
- `searchAll(query: String!, ...)` — Full-archive search (requires Elevated+ access)
- `user(id: ID!)` — Look up user by ID
- `userByUsername(username: String!)` — Look up user by username
- `users(ids: [ID!]!)` — Batch look up users by ID
- `usersByUsernames(usernames: [String!]!)` — Batch look up users by username
- `userTimeline(userId: ID!, ...)` — Get a user's posted tweets
- `userMentionsTimeline(userId: ID!, ...)` — Get tweets mentioning a user
- `userLikedTweets(userId: ID!, ...)` — Get tweets liked by a user
- `userFollowers(userId: ID!, ...)` — Get a user's followers
- `userFollowing(userId: ID!, ...)` — Get users a user follows
- `userBlockedUsers(userId: ID!, ...)` — Get a user's blocked users
- `userMutedUsers(userId: ID!, ...)` — Get a user's muted users
- `userBookmarks(userId: ID!, ...)` — Get a user's bookmarked tweets
- `list(id: ID!)` — Look up a List by ID
- `lists(userId: ID!, ...)` — Get lists owned/followed by a user
- `listMembers(listId: ID!, ...)` — Get members of a list
- `listFollowers(listId: ID!, ...)` — Get followers of a list
- `listTweets(listId: ID!, ...)` — Get tweets from a list
- `space(id: ID!)` — Look up a Space by ID
- `spaces(ids: [ID!]!)` — Batch look up Spaces
- `spacesByCreators(userIds: [ID!]!)` — Get Spaces by creator
- `trends(woeid: Int)` — Get trending topics
- `streamRules` — Get current filtered stream rules
- `usageStats` — Get API usage statistics

## Mutation Operations

- `createTweet(input: CreateTweetInput!)` — Post a new tweet
- `deleteTweet(id: ID!)` — Delete a tweet
- `likeTweet(userId: ID!, tweetId: ID!)` — Like a tweet
- `unlikeTweet(userId: ID!, tweetId: ID!)` — Remove a like
- `retweet(userId: ID!, tweetId: ID!)` — Retweet
- `deleteRetweet(userId: ID!, sourceTweetId: ID!)` — Undo a retweet
- `bookmarkTweet(userId: ID!, tweetId: ID!)` — Bookmark a tweet
- `deleteBookmark(userId: ID!, tweetId: ID!)` — Remove a bookmark
- `followUser(userId: ID!, targetUserId: ID!)` — Follow a user
- `unfollowUser(userId: ID!, targetUserId: ID!)` — Unfollow a user
- `blockUser(userId: ID!, targetUserId: ID!)` — Block a user
- `unblockUser(userId: ID!, targetUserId: ID!)` — Unblock a user
- `muteUser(userId: ID!, targetUserId: ID!)` — Mute a user
- `unmuteUser(userId: ID!, targetUserId: ID!)` — Unmute a user
- `createList(input: CreateListInput!)` — Create a list
- `updateList(id: ID!, input: UpdateListInput!)` — Update a list
- `deleteList(id: ID!)` — Delete a list
- `addListMember(listId: ID!, userId: ID!)` — Add a member to a list
- `removeListMember(listId: ID!, userId: ID!)` — Remove a member from a list
- `followList(userId: ID!, listId: ID!)` — Follow a list
- `unfollowList(userId: ID!, listId: ID!)` — Unfollow a list
- `pinList(userId: ID!, listId: ID!)` — Pin a list
- `unpinList(userId: ID!, listId: ID!)` — Unpin a list
- `createStreamRule(input: CreateStreamRuleInput!)` — Add a filtered stream rule
- `deleteStreamRules(ids: [ID!]!)` — Remove filtered stream rules
- `sendDirectMessage(input: SendDirectMessageInput!)` — Send a DM
- `createComplianceJob(input: CreateComplianceJobInput!)` — Start a compliance job

## Subscription Operations

- `filteredStream(rules: [StreamRule!])` — Real-time tweet stream matching rules
- `sampledStream` — 1% random sample of the public tweet stream
- `activityStream(userId: ID!)` — Real-time activity events for a user (Activity API)
