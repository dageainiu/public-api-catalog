# opal-snails API

Fictional trail-map stickers.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/opal-snails`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/opal-snails/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/opal-snails/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/opal-snails/list` | Paginated fictional collection |
| GET | `/v1/opal-snails/opal-snails` | Fictional service summary |
| GET | `/v1/opal-snails/health` | Documentation liveness sample |

## Example

```http
GET /v1/opal-snails/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "opal-snails",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "opal-snails_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
