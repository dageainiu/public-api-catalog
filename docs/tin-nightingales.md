# tin-nightingales API

Fictional music-box serials.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/tin-nightingales`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/tin-nightingales/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/tin-nightingales/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/tin-nightingales/list` | Paginated fictional collection |
| GET | `/v1/tin-nightingales/tin-nightingales` | Fictional service summary |
| GET | `/v1/tin-nightingales/health` | Documentation liveness sample |

## Example

```http
GET /v1/tin-nightingales/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "tin-nightingales",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "tin-nightingales_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
