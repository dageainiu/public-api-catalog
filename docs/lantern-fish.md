# lantern-fish API

Fictional deep-lantern fish sighting cards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/lantern-fish`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/lantern-fish/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/lantern-fish/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/lantern-fish/list` | Paginated fictional collection |
| GET | `/v1/lantern-fish/lantern-fish` | Fictional service summary |
| GET | `/v1/lantern-fish/health` | Documentation liveness sample |

## Example

```http
GET /v1/lantern-fish/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "lantern-fish",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "lantern-fish_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
