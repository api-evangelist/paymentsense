---
name: Take a Pay-At-Counter card payment
description: Drive a Paymentsense Connect card terminal to take an in-person payment from EPOS software, then confirm the outcome.
api: openapi/paymentsense-connect-v2.json
operations: [PACTerminals, TransactionOnTID, GetTransactionWithRequestId, VerifySignature, CancelTransactionWithRequestId]
---

# Take a Pay-At-Counter card payment

Use the Connect REST API v2 (`Accept: application/connect.v2+json`) against the merchant's
per-site host (`https://<host>.connect.paymentsense.cloud`).

## Auth & headers
- `Authorization: Basic <base64(username:API_KEY)>` — the API key is the password, username identifies the EPoS.
- `Software-House-Id` and `Installer-Id` headers are required (issued by Paymentsense).
- `Content-Type: application/json`, `Accept: application/connect.v2+json`.

## Steps
1. **Find the terminal.** `PACTerminals` lists terminals; note the target `tid`.
2. **Start the transaction.** `TransactionOnTID` (POST `/pac/terminals/{tid}/transactions`) with the amount
   and `transactionType` (SALE, REFUND, PRE_AUTH, COMPLETION+authCode, ACCOUNT_VERIFICATION;
   optional `amountCashback`, `cardholderNotPresent`). It returns **202 Accepted** with a `requestId`.
3. **Poll for progress.** Call `GetTransactionWithRequestId` about once per second. Surface any
   `userMessage` to the operator (e.g. `REPLACE_PAPER`, `ENTER_CASHBACK`, terminal-unavailable).
4. **Handle signature if prompted.** If the terminal requests a signature, capture it and call
   `VerifySignature` to approve/reject **within 80 seconds** or it times out.
5. **Cancel if needed.** `CancelTransactionWithRequestId` requests cancellation; watch for
   `ATTEMPTING_CANCEL` / `CANCELLING` / `UNABLE_TO_CANCEL` notification states.

## Rules
- Never assume completion from the 202 — the terminal outcome only arrives via polling/notifications.
- Errors use a `userMessage` string envelope, not RFC 9457 (see errors/paymentsense-problem-types.yml).
- No idempotency key; do not blindly retry a POST after a timeout — poll the `requestId` first.
