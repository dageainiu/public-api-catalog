# nebula-tea API

Fictional tea blends named after invented nebulae.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/nebula-tea`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/nebula-tea/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/nebula-tea/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/nebula-tea/list` | Paginated fictional collection |
| GET | `/v1/nebula-tea/nebula-tea` | Fictional service summary |
| GET | `/v1/nebula-tea/health` | Documentation liveness sample |

## Example

```http
GET /v1/nebula-tea/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "nebula-tea",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "nebula-tea_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
