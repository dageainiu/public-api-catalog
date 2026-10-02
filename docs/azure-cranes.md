# azure-cranes API

Fictional migration postcard index.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/azure-cranes`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/azure-cranes/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/azure-cranes/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/azure-cranes/list` | Paginated fictional collection |
| GET | `/v1/azure-cranes/azure-cranes` | Fictional service summary |
| GET | `/v1/azure-cranes/health` | Documentation liveness sample |

## Example

```http
GET /v1/azure-cranes/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "azure-cranes",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "azure-cranes_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
