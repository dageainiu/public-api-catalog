# ivory-herons API

Fictional marsh lookout shifts.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/ivory-herons`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/ivory-herons/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/ivory-herons/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/ivory-herons/list` | Paginated fictional collection |
| GET | `/v1/ivory-herons/ivory-herons` | Fictional service summary |
| GET | `/v1/ivory-herons/health` | Documentation liveness sample |

## Example

```http
GET /v1/ivory-herons/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "ivory-herons",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "ivory-herons_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
