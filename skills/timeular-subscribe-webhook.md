---
name: Subscribe to time-tracking webhooks
description: Subscribe a target URL to EARLY (Timeular) webhook events and manage subscriptions.
api: openapi/timeular-early-openapi.yml
operations: [signInWithApiKeyApiSecret, listAvailableEvents, subscribe, listSubscriptions, unsubscribe]
---

# Subscribe to time-tracking webhooks

## Auth
1. `signInWithApiKeyApiSecret` — POST `/developer/sign-in`; use the Access Token as `Authorization: Bearer <token>`.

## Steps
1. `listAvailableEvents` — GET `/webhooks/event`. Choose an event (e.g. `trackingStarted`, `timeEntryCreated`, `timeLeaveApproved`).
2. `subscribe` — POST `/webhooks/subscription` with `{ "event": "trackingStarted", "target_url": "https://example.org/hook" }`. The target must be a valid, publicly reachable HTTPS URL.
3. `listSubscriptions` — GET `/webhooks/subscription` to confirm.
4. `unsubscribe` — DELETE `/webhooks/subscription/{id}` to remove one subscription.

## Rules
- Delivery is HTTPS POST with a 10 second timeout.
- If your endpoint returns `410 GONE`, EARLY auto-unsubscribes it.
- 18 event types exist across time entries, tracking, activities, folders, and leave. See webhooks/timeular-early-webhooks.yml.
