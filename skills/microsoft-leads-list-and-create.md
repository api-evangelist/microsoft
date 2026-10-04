---
name: microsoft-leads-list-and-create
description: Retrieve existing leads and add a new lead to the system.
api: openapi/microsoft-leads-api-openapi.yml
operations:
- listLeads
- createLead
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/microsoft-leads-api-openapi.yml ; every operationId checked against the contract
---

# microsoft-leads-list-and-create

Retrieve existing leads and add a new lead to the system.

## Steps

1. 1. Use `listLeads` operation. Required headers: `Authorization` (accessKey), `Ocp-Apim-Subscription-Key` (apiKey), `api-key` (apiKey).
2. 2. Use `createLead` operation. Required headers: `Authorization` (accessKey), `Ocp-Apim-Subscription-Key` (apiKey), `api-key` (apiKey).

## Rules

- Authentication: Include one of the supported auth headers (e.g., `Authorization` for accessKey, `Ocp-Apim-Subscription-Key` or `api-key` for apiKey).
- Idempotency: `createLead` is not idempotent; avoid retrying without ensuring the lead was not already created.
