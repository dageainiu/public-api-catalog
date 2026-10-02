# mist-ferries API

Fictional fog-route timetables.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/mist-ferries`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/mist-ferries/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/mist-ferries/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/mist-ferries/list` | Paginated fictional collection |
| GET | `/v1/mist-ferries/mist-ferries` | Fictional service summary |
| GET | `/v1/mist-ferries/health` | Documentation liveness sample |

## Example

```http
GET /v1/mist-ferries/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "mist-ferries",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "mist-ferries_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
