# undersea-trains API

Fictional abyssal rail lines and station names.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/undersea-trains`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/undersea-trains/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/undersea-trains/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/undersea-trains/list` | Paginated fictional collection |
| GET | `/v1/undersea-trains/undersea-trains` | Fictional service summary |
| GET | `/v1/undersea-trains/health` | Documentation liveness sample |

## Example

```http
GET /v1/undersea-trains/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "undersea-trains",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "undersea-trains_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
