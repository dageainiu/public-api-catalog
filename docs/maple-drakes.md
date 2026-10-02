# maple-drakes API

Fictional autumn wyrm census.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/maple-drakes`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/maple-drakes/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/maple-drakes/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/maple-drakes/list` | Paginated fictional collection |
| GET | `/v1/maple-drakes/maple-drakes` | Fictional service summary |
| GET | `/v1/maple-drakes/health` | Documentation liveness sample |

## Example

```http
GET /v1/maple-drakes/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "maple-drakes",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "maple-drakes_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
