# pebble-golems API

Fictional stack-height permits.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/pebble-golems`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/pebble-golems/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/pebble-golems/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/pebble-golems/list` | Paginated fictional collection |
| GET | `/v1/pebble-golems/pebble-golems` | Fictional service summary |
| GET | `/v1/pebble-golems/health` | Documentation liveness sample |

## Example

```http
GET /v1/pebble-golems/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "pebble-golems",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "pebble-golems_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
