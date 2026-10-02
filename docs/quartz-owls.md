# quartz-owls API

Fictional night-watch roost lists.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/quartz-owls`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/quartz-owls/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/quartz-owls/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/quartz-owls/list` | Paginated fictional collection |
| GET | `/v1/quartz-owls/quartz-owls` | Fictional service summary |
| GET | `/v1/quartz-owls/health` | Documentation liveness sample |

## Example

```http
GET /v1/quartz-owls/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "quartz-owls",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "quartz-owls_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
