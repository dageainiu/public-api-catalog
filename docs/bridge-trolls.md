# bridge-trolls API

Fictional toll-booth shift boards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/bridge-trolls`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/bridge-trolls/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/bridge-trolls/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/bridge-trolls/list` | Paginated fictional collection |
| GET | `/v1/bridge-trolls/bridge-trolls` | Fictional service summary |
| GET | `/v1/bridge-trolls/health` | Documentation liveness sample |

## Example

```http
GET /v1/bridge-trolls/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "bridge-trolls",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "bridge-trolls_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
