# starlight-ink API

Fictional ink bottle lot numbers.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/starlight-ink`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/starlight-ink/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/starlight-ink/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/starlight-ink/list` | Paginated fictional collection |
| GET | `/v1/starlight-ink/starlight-ink` | Fictional service summary |
| GET | `/v1/starlight-ink/health` | Documentation liveness sample |

## Example

```http
GET /v1/starlight-ink/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "starlight-ink",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "starlight-ink_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
