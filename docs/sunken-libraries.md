# sunken-libraries API

Fictional drowned-stack call numbers.

**Fictional.** Sample documentation only. Not a real service, product, or instruction. Host `api.example.invalid` is not live.

Base URL pattern: `https://api.example.invalid/v1/sunken-libraries`

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| GET | `/v1/sunken-libraries/search` | Search fictional records. Query: `q`, `limit`, `offset` |
| GET | `/v1/sunken-libraries/lookup` | Lookup one fictional record by `id` |
| GET | `/v1/sunken-libraries/list` | Paginated fictional collection |
| GET | `/v1/sunken-libraries/sunken-libraries` | Fictional service summary |
| GET | `/v1/sunken-libraries/health` | Documentation liveness sample |

## Example

```http
GET /v1/sunken-libraries/search?q=sample&limit=20 HTTP/1.1
Accept: application/json
```

```json
{
  "service": "sunken-libraries",
  "fictional": true,
  "query": "sample",
  "count": 1,
  "items": [{"id": "sunken-libraries_001", "title": "sample record"}]
}
```

See also [index](../api/index.json) and [OpenAPI](../openapi/catalog.yaml).
