# amber-flies API

Fictional trapped-moment catalog.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/amber-flies`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/amber-flies/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/amber-flies/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/amber-flies/list` | Paginated fictional collection |
| GET | `/v1/amber-flies/amber-flies` | Fictional service summary |
| GET | `/v1/amber-flies/health` | Documentation liveness sample |

## Example

```http
GET /v1/amber-flies/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "amber-flies",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "amber-flies_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
