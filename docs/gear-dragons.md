# gear-dragons API

Fictional mechanical wyrm serials.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/gear-dragons`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/gear-dragons/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/gear-dragons/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/gear-dragons/list` | Paginated fictional collection |
| GET | `/v1/gear-dragons/gear-dragons` | Fictional service summary |
| GET | `/v1/gear-dragons/health` | Documentation liveness sample |

## Example

```http
GET /v1/gear-dragons/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "gear-dragons",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "gear-dragons_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
