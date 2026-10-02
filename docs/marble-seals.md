# marble-seals API

Fictional harbor stamp books.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/marble-seals`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/marble-seals/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/marble-seals/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/marble-seals/list` | Paginated fictional collection |
| GET | `/v1/marble-seals/marble-seals` | Fictional service summary |
| GET | `/v1/marble-seals/health` | Documentation liveness sample |

## Example

```http
GET /v1/marble-seals/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "marble-seals",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "marble-seals_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
