# lighthouse-ghosts API

Fictional keeper shift boards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/lighthouse-ghosts`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/lighthouse-ghosts/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/lighthouse-ghosts/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/lighthouse-ghosts/list` | Paginated fictional collection |
| GET | `/v1/lighthouse-ghosts/lighthouse-ghosts` | Fictional service summary |
| GET | `/v1/lighthouse-ghosts/health` | Documentation liveness sample |

## Example

```http
GET /v1/lighthouse-ghosts/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "lighthouse-ghosts",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "lighthouse-ghosts_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
