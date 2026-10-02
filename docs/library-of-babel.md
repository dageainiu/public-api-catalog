# library-of-babel API

Fictional shelf addresses for invented books.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/library-of-babel`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/library-of-babel/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/library-of-babel/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/library-of-babel/list` | Paginated fictional collection |
| GET | `/v1/library-of-babel/library-of-babel` | Fictional service summary |
| GET | `/v1/library-of-babel/health` | Documentation liveness sample |

## Example

```http
GET /v1/library-of-babel/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "library-of-babel",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "library-of-babel_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
