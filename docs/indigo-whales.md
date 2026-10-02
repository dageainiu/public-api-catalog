# indigo-whales API

Fictional song-catalog identifiers.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/indigo-whales`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/indigo-whales/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/indigo-whales/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/indigo-whales/list` | Paginated fictional collection |
| GET | `/v1/indigo-whales/indigo-whales` | Fictional service summary |
| GET | `/v1/indigo-whales/health` | Documentation liveness sample |

## Example

```http
GET /v1/indigo-whales/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "indigo-whales",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "indigo-whales_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
