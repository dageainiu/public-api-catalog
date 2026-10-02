# cloud-cities API

Fictional cloud-city districts and lift schedules.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/cloud-cities`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/cloud-cities/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/cloud-cities/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/cloud-cities/list` | Paginated fictional collection |
| GET | `/v1/cloud-cities/cloud-cities` | Fictional service summary |
| GET | `/v1/cloud-cities/health` | Documentation liveness sample |

## Example

```http
GET /v1/cloud-cities/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "cloud-cities",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "cloud-cities_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
