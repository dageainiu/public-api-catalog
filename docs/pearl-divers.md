# pearl-divers API

Fictional dive-bell shift cards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/pearl-divers`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/pearl-divers/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/pearl-divers/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/pearl-divers/list` | Paginated fictional collection |
| GET | `/v1/pearl-divers/pearl-divers` | Fictional service summary |
| GET | `/v1/pearl-divers/health` | Documentation liveness sample |

## Example

```http
GET /v1/pearl-divers/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "pearl-divers",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "pearl-divers_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
