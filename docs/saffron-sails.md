# saffron-sails API

Fictional spice-ship manifests.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/saffron-sails`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/saffron-sails/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/saffron-sails/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/saffron-sails/list` | Paginated fictional collection |
| GET | `/v1/saffron-sails/saffron-sails` | Fictional service summary |
| GET | `/v1/saffron-sails/health` | Documentation liveness sample |

## Example

```http
GET /v1/saffron-sails/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "saffron-sails",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "saffron-sails_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
