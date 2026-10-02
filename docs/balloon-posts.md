# balloon-posts API

Fictional airmail balloon routes.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/balloon-posts`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/balloon-posts/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/balloon-posts/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/balloon-posts/list` | Paginated fictional collection |
| GET | `/v1/balloon-posts/balloon-posts` | Fictional service summary |
| GET | `/v1/balloon-posts/health` | Documentation liveness sample |

## Example

```http
GET /v1/balloon-posts/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "balloon-posts",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "balloon-posts_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
