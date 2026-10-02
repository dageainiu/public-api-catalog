# sand-ships API

Fictional desert vessel logs.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/sand-ships`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/sand-ships/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/sand-ships/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/sand-ships/list` | Paginated fictional collection |
| GET | `/v1/sand-ships/sand-ships` | Fictional service summary |
| GET | `/v1/sand-ships/health` | Documentation liveness sample |

## Example

```http
GET /v1/sand-ships/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "sand-ships",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "sand-ships_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
