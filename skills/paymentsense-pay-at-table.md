---
name: Run a Pay-At-Table hospitality flow
description: Open a table, set its amount, take payment and close it using the Paymentsense Connect Pay-At-Table API.
api: openapi/paymentsense-connect-v1.json
operations: [Tables, OpenTable, Table, TableAmount, TableLock, DeleteTable]
---

# Run a Pay-At-Table hospitality flow

Connect Pay-At-Table (`/pat`) lets hospitality EPOS software manage table balances and take payment
at the table. Same auth model as Pay-At-Counter (HTTP Basic + Software-House-Id/Installer-Id headers).

## Steps
1. **List / open the table.** `Tables` shows open tables; `OpenTable` (PUT `/pat/tables`) opens one by name.
2. **Set the amount due.** `TableAmount` (PUT `/pat/tables/{tableName}/amount`) writes the balance.
   A locked table returns **423 Locked** with a `location` string pointing at the lock holder.
3. **Lock while paying.** `TableLock` prevents concurrent edits during payment.
4. **Read state.** `Table` (GET `/pat/tables/{tableName}`) returns the table; each payment carries a
   `paymentId`. Receipt data is excluded unless the `receipt` query parameter is supplied.
5. **Close the table.** `DeleteTable` (DELETE `/pat/tables/{tableName}`) closes it once settled.

## Rules
- Poll table/payment state roughly every 5 seconds (Pay-At-Table cadence).
- Honour 423 Locked — retry after the lock clears rather than forcing writes.
- Surface `userMessage` strings to staff; errors are not RFC 9457.
