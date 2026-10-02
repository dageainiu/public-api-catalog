# frost-gardens API

Fictional glasshouse bed labels.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/frost-gardens`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/frost-gardens/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/frost-gardens/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/frost-gardens/list` | Paginated fictional collection |
| GET | `/v1/frost-gardens/frost-gardens` | Fictional service summary |
| GET | `/v1/frost-gardens/health` | Documentation liveness sample |

## Example

```http
GET /v1/frost-gardens/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "frost-gardens",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "frost-gardens_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
