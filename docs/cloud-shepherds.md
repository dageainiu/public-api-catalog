# cloud-shepherds API

Fictional flock routes across invented skies.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/cloud-shepherds`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/cloud-shepherds/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/cloud-shepherds/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/cloud-shepherds/list` | Paginated fictional collection |
| GET | `/v1/cloud-shepherds/cloud-shepherds` | Fictional service summary |
| GET | `/v1/cloud-shepherds/health` | Documentation liveness sample |

## Example

```http
GET /v1/cloud-shepherds/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "cloud-shepherds",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "cloud-shepherds_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
