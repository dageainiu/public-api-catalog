# comet-mail API

Fictional message capsules on made-up comets.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/comet-mail`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/comet-mail/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/comet-mail/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/comet-mail/list` | Paginated fictional collection |
| GET | `/v1/comet-mail/comet-mail` | Fictional service summary |
| GET | `/v1/comet-mail/health` | Documentation liveness sample |

## Example

```http
GET /v1/comet-mail/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "comet-mail",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "comet-mail_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
