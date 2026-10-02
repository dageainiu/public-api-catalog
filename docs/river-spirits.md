# river-spirits API

Fictional ford crossing permits.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/river-spirits`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/river-spirits/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/river-spirits/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/river-spirits/list` | Paginated fictional collection |
| GET | `/v1/river-spirits/river-spirits` | Fictional service summary |
| GET | `/v1/river-spirits/health` | Documentation liveness sample |

## Example

```http
GET /v1/river-spirits/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "river-spirits",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "river-spirits_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
