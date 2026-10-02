# crystal-caves API

Fictional cavern maps and glow indexes.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/crystal-caves`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/crystal-caves/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/crystal-caves/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/crystal-caves/list` | Paginated fictional collection |
| GET | `/v1/crystal-caves/crystal-caves` | Fictional service summary |
| GET | `/v1/crystal-caves/health` | Documentation liveness sample |

## Example

```http
GET /v1/crystal-caves/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "crystal-caves",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "crystal-caves_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
