# paper-planes API

Fictional folded-craft flight cards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/paper-planes`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/paper-planes/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/paper-planes/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/paper-planes/list` | Paginated fictional collection |
| GET | `/v1/paper-planes/paper-planes` | Fictional service summary |
| GET | `/v1/paper-planes/health` | Documentation liveness sample |

## Example

```http
GET /v1/paper-planes/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "paper-planes",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "paper-planes_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
