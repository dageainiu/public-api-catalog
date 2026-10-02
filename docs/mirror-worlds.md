# mirror-worlds API

Fictional reflection-realm directories.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/mirror-worlds`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/mirror-worlds/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/mirror-worlds/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/mirror-worlds/list` | Paginated fictional collection |
| GET | `/v1/mirror-worlds/mirror-worlds` | Fictional service summary |
| GET | `/v1/mirror-worlds/health` | Documentation liveness sample |

## Example

```http
GET /v1/mirror-worlds/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "mirror-worlds",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "mirror-worlds_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
