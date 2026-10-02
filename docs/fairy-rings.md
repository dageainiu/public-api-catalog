# fairy-rings API

Fictional ring coordinates and visiting hours.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/fairy-rings`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/fairy-rings/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/fairy-rings/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/fairy-rings/list` | Paginated fictional collection |
| GET | `/v1/fairy-rings/fairy-rings` | Fictional service summary |
| GET | `/v1/fairy-rings/health` | Documentation liveness sample |

## Example

```http
GET /v1/fairy-rings/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "fairy-rings",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "fairy-rings_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
