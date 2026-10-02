# ghosts API

Fictional haunting location cards.

**Fictional.** This page is sample documentation only. Nothing here is a real service, product, or instruction. Host `api.example.invalid` does not resolve to a live API.

Base URL pattern: `https://api.example.invalid/v1/ghosts`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/ghosts/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/ghosts/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/ghosts/list` | Paginated fictional collection |
| GET | `/v1/ghosts/ghosts` | Fictional service summary |
| GET | `/v1/ghosts/health` | Documentation liveness sample |

## Example

```http
GET /v1/ghosts/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "ghosts",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "ghosts_001", "title": "sample record"}]
}
```

## Fields

- `id`: stable sample identifier
- `title`: invented label
- `fictional`: always true
- `updated_at`: RFC 3339 sample timestamp

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
