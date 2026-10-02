# willow-lamps API

Fictional riverside lamp routes.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/willow-lamps`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/willow-lamps/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/willow-lamps/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/willow-lamps/list` | Paginated fictional collection |
| GET | `/v1/willow-lamps/willow-lamps` | Fictional service summary |
| GET | `/v1/willow-lamps/health` | Documentation liveness sample |

## Example

```http
GET /v1/willow-lamps/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "willow-lamps",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "willow-lamps_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
