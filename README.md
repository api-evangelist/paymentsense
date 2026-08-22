# Paymentsense (paymentsense)

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

Paymentsense is a United Kingdom payment processing company that provides card payment acceptance to small and medium-sized businesses through card machines (PDQ terminals), online payment gateways, and EPOS integrations. Now part of Dojo, its developer-facing surface centers on the Connect platform, a cloud-hosted integration layer that gives each merchant an isolated host so point-of-sale and hospitality software can drive card terminals without touching card data. Authentication is HTTP Basic using a per-merchant API key supplied by Paymentsense.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/apis.yml)

## Tags

- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Card Payments
- Acquiring
- Point of Sale
- In-Person Payments

## Timestamps

- **Created:** 2026-07-24
- **Modified:** 2026-07-24

## APIs

### Paymentsense Connect REST API

Cloud REST API for driving Paymentsense card terminals from EPOS software. Covers Pay-At-Counter (`/pac`) transactions and reports and Pay-At-Table (`/pat`) hospitality flows against a per-merchant Connect host. Published in versions v0 (Swagger 2.0, 3.0-beta), v1 (Swagger 2.0, 3.1) and v2 (OpenAPI 3.0, 3.2, current). Authenticates with HTTP Basic using the merchant API key as the password.

- **Human URL:** [https://docs.connect.paymentsense.cloud/rest/api](https://docs.connect.paymentsense.cloud/rest/api)
- **Base URL:** `https://your-host-here.connect.paymentsense.cloud`

#### Properties

- [Documentation](https://docs.connect.paymentsense.cloud/rest/getting-started)
- [API Reference](https://docs.connect.paymentsense.cloud/rest/api)
- [OpenAPI (v2, current)](openapi/paymentsense-connect-v2.json)
- [OpenAPI (v1)](openapi/paymentsense-connect-v1.json)
- [OpenAPI (v0)](openapi/paymentsense-connect-v0.json)

### Paymentsense Connect-E REST API

OpenAPI 3.0 REST API for online / e-commerce card payments. Issues access-tokens, processes and resumes payments, runs cross-reference (repeat) payments, and lists supported payment methods against the Connect-E host.

- **Human URL:** [https://docs.connect.paymentsense.cloud/ConnectE/RestApi](https://docs.connect.paymentsense.cloud/ConnectE/RestApi)
- **Base URL:** `https://e.test.connect.paymentsense.cloud`

#### Properties

- [Documentation](https://docs.connect.paymentsense.cloud/ConnectE/RestApi)
- [OpenAPI](openapi/paymentsense-connect-e-v0.json)

### Paymentsense Connect WebSockets API

Documented WebSockets interface for the Connect platform, offering an event-driven alternative to the REST API for terminal integration. No downloadable OpenAPI/AsyncAPI specification is published; only reference documentation is available.

- **Human URL:** [https://docs.connect.paymentsense.cloud/websockets/api](https://docs.connect.paymentsense.cloud/websockets/api)

#### Properties

- [Documentation](https://docs.connect.paymentsense.cloud/websockets/getting-started)
- [API Reference](https://docs.connect.paymentsense.cloud/websockets/api)

## Common Properties

- [Website](https://www.paymentsense.com/uk/)
- [Developer Portal](https://docs.connect.paymentsense.cloud/)
- [Documentation](https://docs.connect.paymentsense.cloud/)
- [API Reference](https://docs.connect.paymentsense.cloud/rest/api)
- [Getting Started](https://docs.connect.paymentsense.cloud/rest/getting-started)
- [GitHub Organization](https://github.com/Paymentsense-DevSupport)
- [Pricing](https://www.paymentsense.com/uk/pricing/)
- [Blog](https://www.paymentsense.com/uk/blog/)
- [Help Center](https://support.paymentsense.com/hc/en-us)
- [Terms of Service](https://www.paymentsense.com/uk/legal/terms/)
- [Privacy Policy](https://www.paymentsense.com/uk/legal/privacy/)
- [LinkedIn](https://www.linkedin.com/company/paymentsense/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
