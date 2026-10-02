# cinder-mice API

Fictional hearth census cards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/cinder-mice`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/cinder-mice/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/cinder-mice/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/cinder-mice/list` | Paginated fictional collection |
| GET | `/v1/cinder-mice/cinder-mice` | Fictional service summary |
| GET | `/v1/cinder-mice/health` | Documentation liveness sample |

## Example

```http
GET /v1/cinder-mice/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "cinder-mice",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "cinder-mice_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
