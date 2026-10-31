# Paymentsense

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

Paymentsense is a United Kingdom payment processing company that provides card payment acceptance to small and medium-sized businesses through card machines (PDQ terminals), online payment gateways, and EPOS integrations. Now part of Dojo, its developer-facing surface centers on the Connect platform, a cloud-hosted integration layer that gives each merchant an isolated host so point-of-sale and hospitality software can drive card terminals without touching card data. Paymentsense publishes a genuine public developer portal at docs.connect.paymentsense.cloud with interactive Swagger reference docs and downloadable OpenAPI/Swagger specifications for the Connect REST API (Pay-At-Counter and Pay-At-Table terminal integration, versions v0/v1/v2) and the Connect-E REST API for online/e-commerce card payments, plus a documented WebSockets interface. Authentication is HTTP Basic using a per-merchant API key supplied by Paymentsense. A separate merchant/software-house management portal at developers.paymentsense.com sits behind Google sign-in.

**Areas:** Payments · United Kingdom · Payment Gateway · Payment Processing · Card Payments · Acquiring · Point-of-Sale · In-Person Payments

## Paymentsense on APIs.io

Everything profiled for Paymentsense is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/paymentsense/](https://apis.io/providers/paymentsense/)** — or go straight to one of the APIs or properties below.

### APIs (18)

- [Paymentsense Connect WebSockets API](https://apis.io/apis/paymentsense/connect-websockets-api/) — Documented WebSockets interface for the Connect platform, offering an event-driven alternative to the REST API for terminal integration. No downloadable…
- [Paymentsense Access Token API](https://apis.io/apis/paymentsense/paymentsense-access-token-api/) — The Access Token API from Paymentsense — 1 operation(s) for access token.
- [Paymentsense Cross Reference Payment API](https://apis.io/apis/paymentsense/paymentsense-cross-reference-payment-api/) — The Cross Reference Payment API from Paymentsense — 1 operation(s) for cross reference payment.
- [Paymentsense Hospitality Reports API](https://apis.io/apis/paymentsense/paymentsense-hospitality-reports-api/) — The Hospitality Reports API from Paymentsense — 2 operation(s) for hospitality reports.
- [Paymentsense Hospitality Tables API](https://apis.io/apis/paymentsense/paymentsense-hospitality-tables-api/) — The Hospitality Tables API from Paymentsense — 6 operation(s) for hospitality tables.
- [Paymentsense PAC Reports API](https://apis.io/apis/paymentsense/paymentsense-pac-reports-api/) — The PAC Reports API from Paymentsense — 2 operation(s) for pac reports.
- [Paymentsense PAC Reports (Ingenico Only) API](https://apis.io/apis/paymentsense/paymentsense-pac-reports-ingenico-only-api/) — The PAC Reports (Ingenico Only) API from Paymentsense — 2 operation(s) for pac reports (ingenico only).
- [Paymentsense PAC Terminals API](https://apis.io/apis/paymentsense/paymentsense-pac-terminals-api/) — The PAC Terminals API from Paymentsense — 3 operation(s) for pac terminals.
- [Paymentsense PAC Transactions API](https://apis.io/apis/paymentsense/paymentsense-pac-transactions-api/) — The PAC Transactions API from Paymentsense — 6 operation(s) for pac transactions.
- [Paymentsense PAT Reports API](https://apis.io/apis/paymentsense/paymentsense-pat-reports-api/) — The PAT Reports API from Paymentsense — 2 operation(s) for pat reports.
- [Paymentsense PAT Tables API](https://apis.io/apis/paymentsense/paymentsense-pat-tables-api/) — The PAT Tables API from Paymentsense — 6 operation(s) for pat tables.
- [Paymentsense Payment Details API](https://apis.io/apis/paymentsense/paymentsense-payment-details-api/) — The Payment Details API from Paymentsense — 1 operation(s) for payment details.
- [Paymentsense Payment Methods API](https://apis.io/apis/paymentsense/paymentsense-payment-methods-api/) — The Payment Methods API from Paymentsense — 1 operation(s) for payment methods.
- [Paymentsense Resume Payment API](https://apis.io/apis/paymentsense/paymentsense-resume-payment-api/) — The Resume Payment API from Paymentsense — 1 operation(s) for resume payment.
- [Paymentsense Retail Reports API](https://apis.io/apis/paymentsense/paymentsense-retail-reports-api/) — The Retail Reports API from Paymentsense — 2 operation(s) for retail reports.
- [Paymentsense Retail Terminals API](https://apis.io/apis/paymentsense/paymentsense-retail-terminals-api/) — The Retail Terminals API from Paymentsense — 2 operation(s) for retail terminals.
- [Paymentsense Retail Transactions API](https://apis.io/apis/paymentsense/paymentsense-retail-transactions-api/) — The Retail Transactions API from Paymentsense — 3 operation(s) for retail transactions.
- [Paymentsense Revoke Access Token API](https://apis.io/apis/paymentsense/paymentsense-revoke-access-token-api/) — The Revoke Access Token API from Paymentsense — 1 operation(s) for revoke access token.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (1)

Multi-step workflows that chain operations into a business task.

- [Paymentsense Pay-At-Counter — take a card payment](https://apis.io/arazzos/paymentsense/paymentsense-pac-take-payment/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Paymentsense Connect Events](https://apis.io/asyncapis/paymentsense/paymentsense-connect-events/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [paymentsense-connect](https://apis.io/servers/paymentsense/paymentsense-connect/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Paymentsense Agentic Access](https://apis.io/agentic-access/paymentsense/paymentsense-agentic-access/)

#### Collections (4)

Postman and Open Collection request collections.

- [Connect-E Development Environment](https://apis.io/collections/paymentsense/open-paymentsense-connect-e-v0/)
- [Connect REST API](https://apis.io/collections/paymentsense/open-paymentsense-connect-v0/)
- [Connect REST API](https://apis.io/collections/paymentsense/open-paymentsense-connect-v1/)
- [Connect REST API](https://apis.io/collections/paymentsense/open-paymentsense-connect-v2/)

#### Overlays (4)

OpenAPI overlays, including conversational phrasing for each operation.

- [Paymentsense Connect E V0 Overlay](https://apis.io/overlays/paymentsense/paymentsense-connect-e-v0-overlay/)
- [Paymentsense Connect V0 Overlay](https://apis.io/overlays/paymentsense/paymentsense-connect-v0-overlay/)
- [Paymentsense Connect V1 Overlay](https://apis.io/overlays/paymentsense/paymentsense-connect-v1-overlay/)
- [Paymentsense Connect V2 Overlay](https://apis.io/overlays/paymentsense/paymentsense-connect-v2-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Paymentsense Authentication](https://apis.io/security/paymentsense/paymentsense-authentication/)
- [Paymentsense Domain Security](https://apis.io/security/paymentsense/paymentsense-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.paymentsense.com/uk/)
- [Documentation](https://docs.connect.paymentsense.cloud/)
- [Getting started](https://docs.connect.paymentsense.cloud/rest/getting-started)
- [API reference](https://docs.connect.paymentsense.cloud/rest/api)
- [Pricing](https://www.paymentsense.com/uk/pricing/)
- [Changelog](https://docs.connect.paymentsense.cloud/rest/changelog)
- [Blog](https://www.paymentsense.com/uk/blog/)
- [Compliance](https://dojo.tech/articles/what-is-pci-compliance/)
- [Terms of service](https://www.paymentsense.com/uk/legal/terms/)
- [Privacy policy](https://www.paymentsense.com/uk/legal/privacy/)
- [GitHub](https://github.com/Paymentsense-DevSupport)
- [Status](https://status.paymentsense.com/)

## API Evangelist rating

**Kin Score 55.1** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 59.6 |
| Contract governance | 18.2 |
| Operational transparency | 42.1 |
| Developer ergonomics | 66.1 |
| Access clarity | 46.1 |

**Agent readiness 26.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
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
| Pagination Ratio | na |
| Operation Distinctiveness | — |

**Regulatory alignment 39.3** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/paymentsense/](https://apis.io/providers/paymentsense/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Paymentsense: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/paymentsense/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
