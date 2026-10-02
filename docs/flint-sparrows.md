# flint-sparrows API

Fictional spark-nest inventories.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/flint-sparrows`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/flint-sparrows/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/flint-sparrows/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/flint-sparrows/list` | Paginated fictional collection |
| GET | `/v1/flint-sparrows/flint-sparrows` | Fictional service summary |
| GET | `/v1/flint-sparrows/health` | Documentation liveness sample |

## Example

```http
GET /v1/flint-sparrows/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "flint-sparrows",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "flint-sparrows_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
