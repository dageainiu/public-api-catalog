# moon-rabbits API

Fictional lunar hare census cards.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/moon-rabbits`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/moon-rabbits/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/moon-rabbits/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/moon-rabbits/list` | Paginated fictional collection |
| GET | `/v1/moon-rabbits/moon-rabbits` | Fictional service summary |
| GET | `/v1/moon-rabbits/health` | Documentation liveness sample |

## Example

```http
GET /v1/moon-rabbits/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "moon-rabbits",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "moon-rabbits_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
