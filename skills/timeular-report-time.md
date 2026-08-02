---
name: Report time over a date range
description: Retrieve time entries and generate a report for a date range using the EARLY (Timeular) Public API.
api: openapi/timeular-early-openapi.yml
operations: [signInWithApiKeyApiSecret, findTimeEntriesInGivenRange, generateReport]
---

# Report time over a date range

## Auth
1. `signInWithApiKeyApiSecret` — POST `/developer/sign-in`; use the Access Token as `Authorization: Bearer <token>`.

## Steps
1. `findTimeEntriesInGivenRange` — GET `/time-entries/{start}/{end}` where `start` and `end` are ISO-8601 timestamps without offset (e.g. `/time-entries/2016-01-01T00:00:00.000/2017-12-31T23:59:59.999`). Returns the entries in range.
2. `generateReport` — POST `/report` to produce a report over the desired period.

## Rules
- The range is expressed in the path, not as cursor/offset pagination.
- An invalid or inverted range returns `400`.
- See conventions/timeular-conventions.yml (pagination = date-range).
