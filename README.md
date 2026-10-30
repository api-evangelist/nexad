# Nexad

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

Nexad (About Intelligence, Inc.) is an AI-native advertising company backed by Andreessen Horowitz, Point72 and Prosus. It ships the Nexad Android Ads SDK — a Java/Kotlin library for embedding contextual, native, WebView, chat-message, and modal-overlay ads directly into mobile and AI-chat applications — and operates Soku AI, an autonomous marketing agent (the NexStudio API at api.soku.ai) that runs and optimizes ad campaigns across Google, Meta, TikTok, and ChatGPT Ads on a 24/7 perceive–decide–act loop with human-in-the-loop approvals. Developers integrate via the Android SDK, the Soku CLI (@soku-ai/cli) for shell-based AI agents such as Claude Code, Codex, and Cursor, an authenticated MCP endpoint at api.soku.ai/mcp, and an open-source marketing skills hub. Nexad publishes no OpenAPI, but it does ship an unusually complete machine-readable substitute: a 281-action capability registry (18 namespaces) in its public MIT-licensed soku-cli repository, where every action declares typed inputs, an output shape, a read/write/risk mode and a requires_review flag — 124 of the 281 actions are human-approval-gated at runtime.

**Areas:** Company · Artificial Intelligence · Advertising · Marketing · Marketing Automation · Contextual Advertising · Mobile SDK · Agents

## Nexad on APIs.io

Everything profiled for Nexad is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/nexad/](https://apis.io/providers/nexad/)** — or go straight to one of the APIs or properties below.

### APIs (2)

- [Nexad Android Ads SDK](https://apis.io/apis/nexad/nexad-android-ads-sdk/) — Java/Kotlin Android SDK for monetizing apps with native, WebView, chat-message, and modal-overlay ad formats — including contextual ads for AI-chat…
- [Soku (NexStudio) API](https://apis.io/apis/nexad/soku-nexstudio-api/) — The Soku AI platform API (identifies as "NexStudio API"). Powers an autonomous marketing agent across ads, analytics (GA4, GSC, PostHog), SEO hosting, and…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [soku](https://apis.io/servers/nexad/soku/)

#### Agent skills (1)

Agent skills built on the API.

- [soku](https://apis.io/agent-skills/nexad/soku/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Nexad Agentic Access](https://apis.io/agentic-access/nexad/nexad-agentic-access/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Nexad Authentication](https://apis.io/security/nexad/nexad-authentication/)
- [Nexad Domain Security](https://apis.io/security/nexad/nexad-domain-security/)
- [Nexad Vulnerability Disclosure](https://apis.io/security/nexad/nexad-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Nexad Plans Pricing](https://apis.io/plans/nexad/nexad-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Nexad Rate Limits](https://apis.io/rate-limits/nexad/nexad-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://nex.ad)
- [Documentation](https://soku.ai/docs)
- [Getting started](https://docs.nex.ad/docs/android/getting-started)
- [API reference](https://docs.nex.ad/docs/android/intro)
- [Pricing](https://soku.ai/pricing)
- [Sign up](https://soku.ai/sign-up)
- [Support](https://join.slack.com/t/soku-talk/shared_invite/zt-3s9i1a4w7-AWlkU3GAiar3wJM4ToYLEg)
- [Changelog](https://soku.ai/changelog)
- [Blog](https://soku.ai/blog)
- [Security](https://github.com/About-Intelligence/soku-cli/blob/main/SECURITY.md)
- [Terms of service](https://soku.ai/terms)
- [Privacy policy](https://soku.ai/privacy)
- [GitHub](https://github.com/About-Intelligence)

## API Evangelist rating

**Kin Score 45.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 66.7 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 28.9 |
| Developer ergonomics | 78.6 |
| Access clarity | 76.3 |

**Agent readiness 38.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 28.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/nexad/](https://apis.io/providers/nexad/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Nexad: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/nexad/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
