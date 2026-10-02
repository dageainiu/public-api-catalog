# mech-hangars API

Fictional walker bay assignments.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/mech-hangars`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/mech-hangars/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/mech-hangars/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/mech-hangars/list` | Paginated fictional collection |
| GET | `/v1/mech-hangars/mech-hangars` | Fictional service summary |
| GET | `/v1/mech-hangars/health` | Documentation liveness sample |

## Example

```http
GET /v1/mech-hangars/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "mech-hangars",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "mech-hangars_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
