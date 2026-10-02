# honey-comets API

Fictional pastry-comet delivery slips.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/honey-comets`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/honey-comets/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/honey-comets/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/honey-comets/list` | Paginated fictional collection |
| GET | `/v1/honey-comets/honey-comets` | Fictional service summary |
| GET | `/v1/honey-comets/health` | Documentation liveness sample |

## Example

```http
GET /v1/honey-comets/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "honey-comets",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "honey-comets_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
