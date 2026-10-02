# volcano-forges API

Fictional caldera workshop slips.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/volcano-forges`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/volcano-forges/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/volcano-forges/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/volcano-forges/list` | Paginated fictional collection |
| GET | `/v1/volcano-forges/volcano-forges` | Fictional service summary |
| GET | `/v1/volcano-forges/health` | Documentation liveness sample |

## Example

```http
GET /v1/volcano-forges/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "volcano-forges",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "volcano-forges_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
