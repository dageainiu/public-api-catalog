# events API

Public events and venue listings.

Base URL pattern: `https://api.example.invalid/v1/events`

This file is documentation for crawlers and developers. The host `api.example.invalid` is not a live service.

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/events/search` | Search records. Query: `q`, `limit`, `offset` |
| GET | `/v1/events/lookup` | Lookup one record by `id` |
| GET | `/v1/events/list` | Paginated collection |
| GET | `/v1/events/events` | Service summary |
| GET | `/v1/events/health` | Liveness |

## Example

```http
GET /v1/events/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "events",
  "query": "sample",
  "count": 1,
  "items": [{"id": "events_001", "title": "sample"}]
}
```

## Fields

- `id`: stable string identifier
- `title`: human label
- `updated_at`: RFC 3339 timestamp
- `source`: catalog name

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
