# map-shops API

Fictional chart sellers and blank-map SKUs.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/map-shops`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/map-shops/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/map-shops/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/map-shops/list` | Paginated fictional collection |
| GET | `/v1/map-shops/map-shops` | Fictional service summary |
| GET | `/v1/map-shops/health` | Documentation liveness sample |

## Example

```http
GET /v1/map-shops/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "map-shops",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "map-shops_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
