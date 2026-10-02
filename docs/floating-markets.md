# floating-markets API

Fictional barge vendor lists.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/floating-markets`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/floating-markets/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/floating-markets/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/floating-markets/list` | Paginated fictional collection |
| GET | `/v1/floating-markets/floating-markets` | Fictional service summary |
| GET | `/v1/floating-markets/health` | Documentation liveness sample |

## Example

```http
GET /v1/floating-markets/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "floating-markets",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "floating-markets_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
