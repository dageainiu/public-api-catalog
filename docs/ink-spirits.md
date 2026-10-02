# ink-spirits API

Fictional manuscript familiars.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/ink-spirits`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/ink-spirits/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/ink-spirits/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/ink-spirits/list` | Paginated fictional collection |
| GET | `/v1/ink-spirits/ink-spirits` | Fictional service summary |
| GET | `/v1/ink-spirits/health` | Documentation liveness sample |

## Example

```http
GET /v1/ink-spirits/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "ink-spirits",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "ink-spirits_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
