# asteroid-motels API

Fictional roadside lodging on fictional rocks.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/asteroid-motels`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/asteroid-motels/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/asteroid-motels/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/asteroid-motels/list` | Paginated fictional collection |
| GET | `/v1/asteroid-motels/asteroid-motels` | Fictional service summary |
| GET | `/v1/asteroid-motels/health` | Documentation liveness sample |

## Example

```http
GET /v1/asteroid-motels/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "asteroid-motels",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "asteroid-motels_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
