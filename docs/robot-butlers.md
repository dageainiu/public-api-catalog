# robot-butlers API

Fictional household automaton nameplates.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/robot-butlers`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/robot-butlers/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/robot-butlers/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/robot-butlers/list` | Paginated fictional collection |
| GET | `/v1/robot-butlers/robot-butlers` | Fictional service summary |
| GET | `/v1/robot-butlers/health` | Documentation liveness sample |

## Example

```http
GET /v1/robot-butlers/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "robot-butlers",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "robot-butlers_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
