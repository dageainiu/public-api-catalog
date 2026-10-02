# oracle API

Fictional prophecy lookups, clearly non-predictive sample text.

**Fictional.** This page is sample documentation only. Nothing here is a real service, product, or instruction. Host `api.example.invalid` does not resolve to a live API.

Base URL pattern: `https://api.example.invalid/v1/oracle`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/oracle/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/oracle/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/oracle/list` | Paginated fictional collection |
| GET | `/v1/oracle/oracle` | Fictional service summary |
| GET | `/v1/oracle/health` | Documentation liveness sample |

## Example

```http
GET /v1/oracle/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "oracle",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "oracle_001", "title": "sample record"}]
}
```

## Fields

- `id`: stable sample identifier
- `title`: invented label
- `fictional`: always true
- `updated_at`: RFC 3339 sample timestamp

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
