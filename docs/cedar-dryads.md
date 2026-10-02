# cedar-dryads API

Fictional grove tenancy cards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/cedar-dryads`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/cedar-dryads/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/cedar-dryads/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/cedar-dryads/list` | Paginated fictional collection |
| GET | `/v1/cedar-dryads/cedar-dryads` | Fictional service summary |
| GET | `/v1/cedar-dryads/health` | Documentation liveness sample |

## Example

```http
GET /v1/cedar-dryads/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "cedar-dryads",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "cedar-dryads_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
