# clockwork API

Fictional gear catalogs and winding intervals.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/clockwork`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/clockwork/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/clockwork/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/clockwork/list` | Paginated fictional collection |
| GET | `/v1/clockwork/clockwork` | Fictional service summary |
| GET | `/v1/clockwork/health` | Documentation liveness sample |

## Example

```http
GET /v1/clockwork/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "clockwork",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "clockwork_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
