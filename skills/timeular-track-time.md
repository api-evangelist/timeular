---
name: Track time with a live session
description: Start and stop a live time-tracking session for an activity using the EARLY (Timeular) Public API.
api: openapi/timeular-early-openapi.yml
operations: [signInWithApiKeyApiSecret, listAllActivities, showCurrentTracking, startTracking, stopTracking]
---

# Track time with a live session

Use the EARLY (Timeular) Public API (base URL `https://api.early.app/api/v4`) to run a live tracking session.

## Auth
1. `signInWithApiKeyApiSecret` — POST `/developer/sign-in` with `{ "apiKey": "...", "apiSecret": "..." }`. Generate the key/secret in the EARLY web app (product.early.app). The response returns an Access Token.
2. Send `Authorization: Bearer <token>` on every subsequent call.

## Steps
1. `listAllActivities` — GET `/activities`. Pick the `id` of the activity to track.
2. `showCurrentTracking` — GET `/tracking`. Confirm nothing is already running (starting while a session is active can return `409 Conflict`).
3. `startTracking` — POST `/tracking/{activityId}/start`. Begins the live session.
4. When done, `stopTracking` — POST `/tracking/stop`. This closes the session and creates the corresponding time entry.

## Rules
- The Access Token is short-lived; on `401` re-run `signInWithApiKeyApiSecret`.
- There is no idempotency key — do not blindly retry `startTracking`; check `showCurrentTracking` first.
- See conventions/timeular-conventions.yml and errors/timeular-problem-types.yml.
