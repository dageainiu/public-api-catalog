# crimson-kites API

Fictional festival kite registrations.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/crimson-kites`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/crimson-kites/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/crimson-kites/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/crimson-kites/list` | Paginated fictional collection |
| GET | `/v1/crimson-kites/crimson-kites` | Fictional service summary |
| GET | `/v1/crimson-kites/health` | Documentation liveness sample |

## Example

```http
GET /v1/crimson-kites/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "crimson-kites",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "crimson-kites_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
