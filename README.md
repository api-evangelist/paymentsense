# Paymentsense (paymentsense)

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
