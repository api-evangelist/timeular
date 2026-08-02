---
name: Create and tag a time entry
description: Create a time entry for a past interval and attach tags using the EARLY (Timeular) Public API.
api: openapi/timeular-early-openapi.yml
operations: [signInWithApiKeyApiSecret, listAllActivities, fetchTagsMentions, createTag, createTimeEntry]
---

# Create and tag a time entry

Log a completed interval directly (rather than running a live session).

## Auth
1. `signInWithApiKeyApiSecret` — POST `/developer/sign-in`; use the returned Access Token as `Authorization: Bearer <token>`.

## Steps
1. `listAllActivities` — GET `/activities`. Choose the activity `id`.
2. `fetchTagsMentions` — GET `/tags-and-mentions`. Find existing tags; if the tag you need is missing, `createTag` — POST `/tags`.
3. `createTimeEntry` — POST `/time-entries` with the activity id, a `startedAt`/`stoppedAt` interval (ISO-8601 without offset, e.g. `2016-01-01T00:00:00.000`), and any tags/mentions.

## Rules
- Timestamps are ISO-8601 without a timezone offset.
- Validation failures return `400`; a missing activity/tag returns `404`.
- Not idempotent — a repeated POST creates a duplicate entry.
- See conventions/timeular-conventions.yml and data-model/timeular-data-model.yml.
