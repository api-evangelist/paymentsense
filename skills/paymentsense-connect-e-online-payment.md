---
name: Take an online card payment with Connect-E
description: Mint a Connect-E access token, collect card data client-side, and take an online payment (incl. 3-D Secure and repeat payments).
api: openapi/paymentsense-connect-e-v0.json
operations: ["/v1/access-tokens", "/v1/payments/", "/v1/payments/resume", "/v1/cross-reference-payments/access-token"]
---

# Take an online card payment with Connect-E

Connect-E is the e-commerce surface (a CyberSource proxy). Card data is captured **client-side** by the
Connect-E JavaScript so your server stays out of PCI scope.

## Auth
- Server calls are secured with a JWT: `Authorization: Bearer <JWT>`.
- Mint a single-use, 30-minute **access token** with `POST /v1/access-tokens` (operationId `/v1/access-tokens`).

## Steps
1. **Create an access token.** `POST /v1/access-tokens` with the amount, currency and a **unique**
   `merchantTransactionId`. The token is single-use and expires in 30 minutes.
2. **Collect the card client-side.** Load `client.js` (test: `web.e.test.connect.paymentsense.cloud`,
   live: `web.e.connect.paymentsense.cloud`) and render **Connect-E Standard** (styleable fields) or
   **Connect-E Checkout** (drop-in). Pass the access token; the browser submits card data to Paymentsense.
3. **Handle 3-D Secure.** For 3DS / 3DS2 challenges, resume with `POST /v1/payments/{access-token}/resume`
   (operationId `/v1/payments/resume`).
4. **Read the result.** `GET /v1/payments/{access-token}` (operationId `/v1/payments/`) returns the outcome.
5. **Repeat / cardholder-not-present payments.** Use
   `POST /v1/cross-reference-payments/{access-token}` (operationId `/v1/cross-reference-payments/access-token`).

## Rules
- `merchantTransactionId` must be unique per payment — it is the duplicate-detection key (no idempotency header).
- Test with the published sandbox cards (see sandbox/paymentsense-sandbox.yml); never use live PANs in test.
- Supported methods are listed at `GET /v1/payment-methods`.
