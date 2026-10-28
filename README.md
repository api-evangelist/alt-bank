# Alt Bank

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

alt.bank (Alt Bank) is a Brazilian fintech providing a fully integrated, turnkey credit-card and consumer-credit platform for partners who want to launch prepaid and postpaid cards without becoming a financial institution. Its flagship product, GUARD, is a machine-learning underwriting / credit-risk engine ("Brazil's most accurate credit model") that returns a Guard Score, risk band and credit-limit decision through a real-time partner API. The platform also bundles white-label credit cards (novücard), Visa BIN sponsorship, KYC, anti-fraud, dispute management and Pix/boleto payment processing. Partners integrate over a documented HTTPS API secured with a per-partner X-Partner-Auth token plus IP allow-listing, with a mirrored staging sandbox and asynchronous callback delivery of underwriting results. Backed by Anthemis, Union Square Ventures, Repeat Ventures and SquareOne Capital, alt.bank targets financial inclusion for underbanked consumers.

**Areas:** Company · Fintech · Banking · Credit · Underwriting · Credit Cards · Payments · KYC · Risk Management · Brazil · Financial Inclusion · Banking as a Service

## Alt Bank on APIs.io

Everything profiled for Alt Bank is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/alt-bank/](https://apis.io/providers/alt-bank/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [GUARD API](https://apis.io/apis/alt-bank/guard-api/) — Real-time consumer credit underwriting / risk-assessment API. Partners POST an underwriting request for a credit-card applicant and receive a Guard Score,…
- [CC Integration API](https://apis.io/apis/alt-bank/cc-integration-api/) — Credit-card module integration API (private, partner B2B) for issuing and managing alt.bank white-label credit cards.
- [SDK KYC API](https://apis.io/apis/alt-bank/sdk-kyc-api/) — Identity verification / KYC SDK and API for onboarding and verifying applicants as part of the alt.bank credit and card flows.
- [Alt Bank Underwriting API](https://apis.io/apis/alt-bank/alt-bank-underwriting-api/) — Credit underwriting and risk scoring for partner card issuance.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Alt Bank Guard Webhooks](https://apis.io/asyncapis/alt-bank/alt-bank-guard-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [alt-bank](https://apis.io/servers/alt-bank/alt-bank/)

#### Collections (1)

Postman and Open Collection request collections.

- [alt.bank GUARD Underwriting API](https://apis.io/collections/alt-bank/open-alt-bank-underwriting-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Alt Bank Authentication](https://apis.io/security/alt-bank/alt-bank-authentication/)
- [Alt Bank Domain Security](https://apis.io/security/alt-bank/alt-bank-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://altbank.ai/en/)
- [Documentation](https://developers.altbank.ai/docs/guard-api)
- [Getting started](https://developers.altbank.ai/docs/getting-started)
- [API reference](https://developers.altbank.ai/docs/guard)
- [Support](https://altbank.ai/en/contact-us/)

## API Evangelist rating

**Kin Score 23.5** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 64.3 |
| Contract quality | 57.6 |
| Contract governance | 0.0 |
| Operational transparency | 7.9 |
| Developer ergonomics | 18.5 |
| Access clarity | 0.0 |

**Agent readiness 20.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 10.7** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/alt-bank/](https://apis.io/providers/alt-bank/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Alt Bank: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/alt-bank/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
