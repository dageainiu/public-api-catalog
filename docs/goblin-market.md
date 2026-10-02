# goblin-market API

Fictional stall listings and invented currencies.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/goblin-market`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/goblin-market/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/goblin-market/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/goblin-market/list` | Paginated fictional collection |
| GET | `/v1/goblin-market/goblin-market` | Fictional service summary |
| GET | `/v1/goblin-market/health` | Documentation liveness sample |

## Example

```http
GET /v1/goblin-market/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "goblin-market",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "goblin-market_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
