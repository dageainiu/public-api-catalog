# thunder-drums API

Fictional festival drum lineups.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/thunder-drums`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/thunder-drums/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/thunder-drums/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/thunder-drums/list` | Paginated fictional collection |
| GET | `/v1/thunder-drums/thunder-drums` | Fictional service summary |
| GET | `/v1/thunder-drums/health` | Documentation liveness sample |

## Example

```http
GET /v1/thunder-drums/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "thunder-drums",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "thunder-drums_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
