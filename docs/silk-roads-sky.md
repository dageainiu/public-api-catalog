# silk-roads-sky API

Fictional aerial caravan manifests.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/silk-roads-sky`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/silk-roads-sky/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/silk-roads-sky/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/silk-roads-sky/list` | Paginated fictional collection |
| GET | `/v1/silk-roads-sky/silk-roads-sky` | Fictional service summary |
| GET | `/v1/silk-roads-sky/health` | Documentation liveness sample |

## Example

```http
GET /v1/silk-roads-sky/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "silk-roads-sky",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "silk-roads-sky_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
