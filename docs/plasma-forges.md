# plasma-forges API

Fictional forge queue tickets.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/plasma-forges`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/plasma-forges/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/plasma-forges/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/plasma-forges/list` | Paginated fictional collection |
| GET | `/v1/plasma-forges/plasma-forges` | Fictional service summary |
| GET | `/v1/plasma-forges/health` | Documentation liveness sample |

## Example

```http
GET /v1/plasma-forges/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "plasma-forges",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "plasma-forges_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
