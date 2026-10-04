---
name: microsoft-manage-list-items
description: Create, retrieve, update, and delete items in a Microsoft List.
api: openapi/microsoft-items-api-openapi.yml
operations:
- listItems
- createListItem
- getListItem
- updateListItem
- deleteListItem
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/microsoft-items-api-openapi.yml ; every operationId checked against the contract
---

# microsoft-manage-list-items

Create, retrieve, update, and delete items in a Microsoft List.

## Steps

1. 1. `listItems` – requires header `Authorization` (accessKey) or `Ocp-Apim-Subscription-Key` (apiKey) or `api-key` (apiKey) and query parameter `listTitle`.
2. 2. `createListItem` – requires header `Authorization` (accessKey) or `Ocp-Apim-Subscription-Key` (apiKey) or `api-key` (apiKey) and body fields for the new item.
3. 3. `getListItem` – requires header `Authorization` (accessKey) or `Ocp-Apim-Subscription-Key` (apiKey) or `api-key` (apiKey) and path parameters `listTitle` and `itemId`.
4. 4. `updateListItem` – requires header `Authorization` (accessKey) or `Ocp-Apim-Subscription-Key` (apiKey) or `api-key` (apiKey) and body fields for the updates, with path parameters `listTitle` and `itemId`.
5. 5. `deleteListItem` – requires header `Authorization` (accessKey) or `Ocp-Apim-Subscription-Key` (apiKey) or `api-key` (apiKey) and path parameters `listTitle` and `itemId`.

## Rules

- Authentication: Provide an `Authorization` header with an access key, or use `Ocp-Apim-Subscription-Key` or `api-key` headers for API key authentication.
- Idempotency: `createListItem` and `updateListItem` are not idempotent; repeat calls may create duplicate items.
- Pagination: Not specified in the provided facts; assume default server pagination if applicable.
- Errors: No specific error codes provided; rely on standard HTTP error responses.
