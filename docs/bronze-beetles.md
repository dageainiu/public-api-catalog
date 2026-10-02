# bronze-beetles API

Fictional clock-beetle winding logs.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/bronze-beetles`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/bronze-beetles/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/bronze-beetles/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/bronze-beetles/list` | Paginated fictional collection |
| GET | `/v1/bronze-beetles/bronze-beetles` | Fictional service summary |
| GET | `/v1/bronze-beetles/health` | Documentation liveness sample |

## Example

```http
GET /v1/bronze-beetles/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "bronze-beetles",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "bronze-beetles_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
