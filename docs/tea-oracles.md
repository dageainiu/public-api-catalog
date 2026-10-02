# tea-oracles API

Fictional leaf-reading ticket stubs.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/tea-oracles`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/tea-oracles/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/tea-oracles/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/tea-oracles/list` | Paginated fictional collection |
| GET | `/v1/tea-oracles/tea-oracles` | Fictional service summary |
| GET | `/v1/tea-oracles/health` | Documentation liveness sample |

## Example

```http
GET /v1/tea-oracles/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "tea-oracles",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "tea-oracles_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
