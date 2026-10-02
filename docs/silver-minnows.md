# silver-minnows API

Fictional stream school counts.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/silver-minnows`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/silver-minnows/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/silver-minnows/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/silver-minnows/list` | Paginated fictional collection |
| GET | `/v1/silver-minnows/silver-minnows` | Fictional service summary |
| GET | `/v1/silver-minnows/health` | Documentation liveness sample |

## Example

```http
GET /v1/silver-minnows/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "silver-minnows",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "silver-minnows_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
