# Public API Catalog

Crawlable index of documented REST endpoints. These pages describe request shapes for a sample public catalog. They are documentation, not live credentials, and they do not collect secrets.

## Machine-readable entry points

- [openapi/catalog.yaml](openapi/catalog.yaml) — OpenAPI 3.1 bundle
- [api/index.json](api/index.json) — endpoint index
- [sitemap.xml](sitemap.xml) — document map
- [llms.txt](llms.txt) — short crawler summary
- [robots.txt](robots.txt) — allows indexing

## Services

- [weather](docs/weather.md) — Weather observations, forecasts, and alerts. Base path `/v1/weather`
- [geo](docs/geo.md) — Geocoding, reverse geocoding, and place search. Base path `/v1/geo`
- [fx](docs/fx.md) — Foreign exchange rates and currency conversion. Base path `/v1/fx`
- [news](docs/news.md) — Headlines, search, and source listings. Base path `/v1/news`
- [books](docs/books.md) — Book metadata, ISBN lookup, and search. Base path `/v1/books`
- [movies](docs/movies.md) — Film metadata, cast, and ratings. Base path `/v1/movies`
- [music](docs/music.md) — Track, album, and artist metadata. Base path `/v1/music`
- [transit](docs/transit.md) — Stops, routes, and arrival estimates. Base path `/v1/transit`
- [flights](docs/flights.md) — Airport status and flight schedules. Base path `/v1/flights`
- [stocks](docs/stocks.md) — Quotes, candles, and symbol search. Base path `/v1/stocks`
- [crypto](docs/crypto.md) — Spot prices and market pairs. Base path `/v1/crypto`
- [translate](docs/translate.md) — Text translation and language detection. Base path `/v1/translate`
- [images](docs/images.md) — Image search and metadata. Base path `/v1/images`
- [nutrition](docs/nutrition.md) — Food search and nutrient lookup. Base path `/v1/nutrition`
- [recipes](docs/recipes.md) — Recipe search and ingredient lists. Base path `/v1/recipes`
- [events](docs/events.md) — Public events and venue listings. Base path `/v1/events`
- [jobs](docs/jobs.md) — Job posting search. Base path `/v1/jobs`
- [holidays](docs/holidays.md) — Public holiday calendars. Base path `/v1/holidays`
- [time](docs/time.md) — Timezone and current time. Base path `/v1/time`
- [ip](docs/ip.md) — IP geolocation lookup. Base path `/v1/ip`
- [dns](docs/dns.md) — DNS record lookup. Base path `/v1/dns`
- [whois](docs/whois.md) — Domain registration lookup. Base path `/v1/whois`
- [packages](docs/packages.md) — Package registry metadata. Base path `/v1/packages`
- [cve](docs/cve.md) — Vulnerability advisory search. Base path `/v1/cve`
- [status](docs/status.md) — Service status pages. Base path `/v1/status`
- [air](docs/air.md) — Air quality indexes. Base path `/v1/air`
- [tides](docs/tides.md) — Tide predictions. Base path `/v1/tides`
- [earthquakes](docs/earthquakes.md) — Seismic event feed. Base path `/v1/earthquakes`
- [space](docs/space.md) — Satellite passes and launches. Base path `/v1/space`
- [sports](docs/sports.md) — Scores and standings. Base path `/v1/sports`
- [dictionary](docs/dictionary.md) — Definitions and synonyms. Base path `/v1/dictionary`
- [quotes](docs/quotes.md) — Attributed quotations. Base path `/v1/quotes`
- [jokes](docs/jokes.md) — Short text jokes. Base path `/v1/jokes`
- [facts](docs/facts.md) — Short factual statements. Base path `/v1/facts`
- [avatars](docs/avatars.md) — Generated avatar metadata. Base path `/v1/avatars`
- [qr](docs/qr.md) — QR payload metadata. Base path `/v1/qr`
- [barcode](docs/barcode.md) — Barcode lookup. Base path `/v1/barcode`
- [zip](docs/zip.md) — Postal code lookup. Base path `/v1/zip`
- [phone](docs/phone.md) — Phone number metadata. Base path `/v1/phone`
- [companies](docs/companies.md) — Company profile lookup. Base path `/v1/companies`

## Common pattern

```
GET /v1/{service}/{resource}
Accept: application/json
```

Query parameters used across the catalog: `q`, `limit`, `offset`, `lang`, `format`.

License: MIT.
