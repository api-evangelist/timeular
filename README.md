# Timeular

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

Timeular (now branded EARLY) is a time-tracking company whose apps and physical tracking device help individuals and teams capture where their time goes. Its public REST API — hosted at api.early.app — lets developers manage activities, start and stop live tracking, create and query time entries over date ranges, generate reports, organize tags and mentions, administer folders, users and leave, and subscribe to webhooks for time-tracking and leave events. Authentication uses an API Key and API Secret exchanged for a short-lived Bearer Access Token. The API is versioned in the URI path (V4 is current; V3 and V2 remain available) and is published as a public Postman collection. Timeular is backed by Speedinvest.

**Areas:** Company · Time Tracking · Productivity · Time Management · Reporting · Team Management · Webhook · Software-as-a-Service

## Timeular on APIs.io

Everything profiled for Timeular is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/timeular/](https://apis.io/providers/timeular/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Timeular Activities API](https://apis.io/apis/timeular/timeular-activities-api/) — The Activities API from Timeular — 3 operation(s) for activities.
- [Timeular Authentication API](https://apis.io/apis/timeular/timeular-authentication-api/) — The Authentication API from Timeular — 3 operation(s) for authentication.
- [Timeular Current Tracking API](https://apis.io/apis/timeular/timeular-current-tracking-api/) — The Current Tracking API from Timeular — 3 operation(s) for current tracking.
- [Timeular Folders API](https://apis.io/apis/timeular/timeular-folders-api/) — The Folders API from Timeular — 4 operation(s) for folders.
- [Timeular Leaves API](https://apis.io/apis/timeular/timeular-leaves-api/) — The Leaves API from Timeular — 6 operation(s) for leaves.
- [Timeular Members API](https://apis.io/apis/timeular/timeular-members-api/) — The Members API from Timeular — 2 operation(s) for members.
- [Timeular Reports API](https://apis.io/apis/timeular/timeular-reports-api/) — The Reports API from Timeular — 1 operation(s) for reports.
- [Timeular Tags & Mentions API](https://apis.io/apis/timeular/timeular-tags-mentions-api/) — The Tags & Mentions API from Timeular — 5 operation(s) for tags & mentions.
- [Timeular Time Entries API](https://apis.io/apis/timeular/timeular-time-entries-api/) — The Time Entries API from Timeular — 3 operation(s) for time entries.
- [Timeular Users API](https://apis.io/apis/timeular/timeular-users-api/) — The Users API from Timeular — 2 operation(s) for users.
- [Timeular Webhooks API](https://apis.io/apis/timeular/timeular-webhooks-api/) — The Webhooks API from Timeular — 3 operation(s) for webhooks.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [EARLY (Timeular) Webhooks](https://apis.io/asyncapis/timeular/timeular-early-asyncapi/)

#### Event channels (5)

Individual events and webhooks the provider emits.

- [activity](https://apis.io/channels/timeular/activity/)
- [folder](https://apis.io/channels/timeular/folder/)
- [timeEntry](https://apis.io/channels/timeular/timeentry/)
- [timeLeave](https://apis.io/channels/timeular/timeleave/)
- [tracking](https://apis.io/channels/timeular/tracking/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [timeular-early](https://apis.io/servers/timeular/timeular-early/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Timeular Agentic Access](https://apis.io/agentic-access/timeular/timeular-agentic-access/)

#### Collections (11)

Postman and Open Collection request collections.

- [EARLY (Timeular) Public Activities API](https://apis.io/collections/timeular/open-timeular-activities-api/)
- [EARLY (Timeular) Public Activities Authentication API](https://apis.io/collections/timeular/open-timeular-authentication-api/)
- [EARLY (Timeular) Public Activities Current Tracking API](https://apis.io/collections/timeular/open-timeular-current-tracking-api/)
- [EARLY (Timeular) Public Activities Folders API](https://apis.io/collections/timeular/open-timeular-folders-api/)
- [EARLY (Timeular) Public Activities Leaves API](https://apis.io/collections/timeular/open-timeular-leaves-api/)
- [EARLY (Timeular) Public Activities Members API](https://apis.io/collections/timeular/open-timeular-members-api/)
- [EARLY (Timeular) Public Activities Reports API](https://apis.io/collections/timeular/open-timeular-reports-api/)
- [EARLY (Timeular) Public Activities Tags & Mentions API](https://apis.io/collections/timeular/open-timeular-tags-mentions-api/)
- [EARLY (Timeular) Public Activities Time Entries API](https://apis.io/collections/timeular/open-timeular-time-entries-api/)
- [EARLY (Timeular) Public Activities Users API](https://apis.io/collections/timeular/open-timeular-users-api/)
- [EARLY (Timeular) Public Activities Webhooks API](https://apis.io/collections/timeular/open-timeular-webhooks-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Timeular Early Overlay](https://apis.io/overlays/timeular/timeular-early-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Timeular Authentication](https://apis.io/security/timeular/timeular-authentication/)
- [Timeular Domain Security](https://apis.io/security/timeular/timeular-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://early.app/)
- [Documentation](https://developers.early.app/)
- [Getting started](https://developers.early.app/)
- [API reference](https://developers.early.app/)
- [Pricing](https://early.app/pricing/)
- [Sign up](https://product.early.app/register)
- [Support](https://support.early.app/en/)
- [Blog](https://early.app/blog/)
- [Privacy policy](https://early.app/privacy-policy/)
- [GitHub](https://github.com/timeular)

## API Evangelist rating

**Kin Score 34.3** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 24.8 |
| Contract governance | 4.5 |
| Operational transparency | 10.5 |
| Developer ergonomics | 63.7 |
| Access clarity | 27.6 |

**Agent readiness 26.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 20.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/timeular/](https://apis.io/providers/timeular/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Timeular: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/timeular/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
