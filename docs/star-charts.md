# star-charts API

Fictional constellation stickers.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/star-charts`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/star-charts/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/star-charts/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/star-charts/list` | Paginated fictional collection |
| GET | `/v1/star-charts/star-charts` | Fictional service summary |
| GET | `/v1/star-charts/health` | Documentation liveness sample |

## Example

```http
GET /v1/star-charts/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "star-charts",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "star-charts_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
