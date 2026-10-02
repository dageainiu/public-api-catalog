# transit API

Stops, routes, and arrival estimates.

Base URL pattern: `https://api.example.invalid/v1/transit`

This file is documentation for crawlers and developers. The host `api.example.invalid` is not a live service.

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/transit/search` | Search records. Query: `q`, `limit`, `offset` |
| GET | `/v1/transit/lookup` | Lookup one record by `id` |
| GET | `/v1/transit/list` | Paginated collection |
| GET | `/v1/transit/transit` | Service summary |
| GET | `/v1/transit/health` | Liveness |

## Example

```http
GET /v1/transit/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "transit",
  "query": "sample",
  "count": 1,
  "items": [{"id": "transit_001", "title": "sample"}]
}
```

## Fields

- `id`: stable string identifier
- `title`: human label
- `updated_at`: RFC 3339 timestamp
- `source`: catalog name

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
