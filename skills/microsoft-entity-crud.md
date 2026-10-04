---
name: microsoft-entity-crud
description: Perform a full CRUD workflow on Entity resources.
api: openapi/microsoft-entities-api-openapi.yml
operations:
- listAccounts
- createAccount
- getAccount
- updateAccount
- deleteAccount
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/microsoft-entities-api-openapi.yml ; every operationId checked against the contract
---

# microsoft-entity-crud

Perform a full CRUD workflow on Entity resources.

## Steps

1. 1. `listAccounts` – requires the `Authorization` header (accessKey) or `Ocp-Apim-Subscription-Key` header (apiKey) or `api-key` header (apiKey).
2. 2. `createAccount` – requires the same authentication headers and a request body with the account fields.
3. 3. `getAccount` – requires the authentication headers and the path parameter `accountid`.
4. 4. `updateAccount` – requires the authentication headers, the path parameter `accountid`, and a request body with the fields to update.
5. 5. `deleteAccount` – requires the authentication headers and the path parameter `accountid`.

## Rules

- Authentication: include one of the supported auth headers – `Authorization` (accessKey), `Ocp-Apim-Subscription-Key` (apiKey), or `api-key` (apiKey).
- Idempotency: `createAccount` and `updateAccount` are not idempotent; repeat calls may create duplicate resources or apply multiple updates.
- Pagination: not specified for these operations; assume default server behavior.
- Error handling: on failure the API returns standard HTTP error codes; no specific rate‑limit headers are defined.
