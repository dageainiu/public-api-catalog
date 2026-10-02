# snow-giants API

Fictional footprint measurement slips.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/snow-giants`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/snow-giants/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/snow-giants/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/snow-giants/list` | Paginated fictional collection |
| GET | `/v1/snow-giants/snow-giants` | Fictional service summary |
| GET | `/v1/snow-giants/health` | Documentation liveness sample |

## Example

```http
GET /v1/snow-giants/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "snow-giants",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "snow-giants_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
