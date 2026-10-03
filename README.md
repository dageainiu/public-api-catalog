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

## Fictional services

These endpoints are invented sample names. They are not real APIs.

- [dragons](docs/dragons.md) — Fictional dragon registry: species, hoard size, and last sighting. Base path `/v1/dragons`
- [time-travel](docs/time-travel.md) — Fictional timeline tickets and paradox warnings. Base path `/v1/time-travel`
- [alchemy](docs/alchemy.md) — Fictional transmutation recipes and reagent inventories. Base path `/v1/alchemy`
- [telepathy](docs/telepathy.md) — Fictional thought-channel session metadata. Base path `/v1/telepathy`
- [portals](docs/portals.md) — Fictional portal coordinates and destination realms. Base path `/v1/portals`
- [dream-log](docs/dream-log.md) — Fictional dream journal entries and symbols. Base path `/v1/dream-log`
- [invisibility](docs/invisibility.md) — Fictional cloak charge levels and duration. Base path `/v1/invisibility`
- [levitation](docs/levitation.md) — Fictional altitude permits and weight limits. Base path `/v1/levitation`
- [oracle](docs/oracle.md) — Fictional prophecy lookups, clearly non-predictive sample text. Base path `/v1/oracle`
- [moonbase](docs/moonbase.md) — Fictional lunar habitat occupancy and airlock status. Base path `/v1/moonbase`
- [kraken](docs/kraken.md) — Fictional sea-monster sighting reports. Base path `/v1/kraken`
- [starship](docs/starship.md) — Fictional vessel registry and jump-drive status. Base path `/v1/starship`
- [hologram](docs/hologram.md) — Fictional hologram scene metadata. Base path `/v1/hologram`
- [cloning](docs/cloning.md) — Fictional clone batch labels, not a biological protocol. Base path `/v1/cloning`
- [weather-control](docs/weather-control.md) — Fictional weather-dial settings for story worlds. Base path `/v1/weather-control`
- [gravity](docs/gravity.md) — Fictional local gravity multipliers. Base path `/v1/gravity`
- [shapeshift](docs/shapeshift.md) — Fictional form catalog and cooldown timers. Base path `/v1/shapeshift`
- [familiars](docs/familiars.md) — Fictional companion creature registry. Base path `/v1/familiars`
- [phoenix](docs/phoenix.md) — Fictional rebirth cycle counters. Base path `/v1/phoenix`
- [merfolk](docs/merfolk.md) — Fictional underwater city directories. Base path `/v1/merfolk`
- [unicorns](docs/unicorns.md) — Fictional grove permits and horn-sparkle indexes. Base path `/v1/unicorns`
- [ghosts](docs/ghosts.md) — Fictional haunting location cards. Base path `/v1/ghosts`
- [potions](docs/potions.md) — Fictional bottle labels and story effects. Base path `/v1/potions`
- [runes](docs/runes.md) — Fictional rune dictionary for invented alphabets. Base path `/v1/runes`
- [wormholes](docs/wormholes.md) — Fictional tunnel maps between made-up systems. Base path `/v1/wormholes`
- [androids](docs/androids.md) — Fictional android serial metadata. Base path `/v1/androids`
- [nanobots](docs/nanobots.md) — Fictional swarm names and story task tags. Base path `/v1/nanobots`
- [cryosleep](docs/cryosleep.md) — Fictional pod occupancy for fictional crews. Base path `/v1/cryosleep`
- [terraforming](docs/terraforming.md) — Fictional planet climate stage labels. Base path `/v1/terraforming`
- [spellbooks](docs/spellbooks.md) — Fictional spell index with invented names only. Base path `/v1/spellbooks`

## More fictional services

- [sky-islands](docs/sky-islands.md) — Fictional floating island registry and dock permits. Base path `/v1/sky-islands`
- [cloud-cities](docs/cloud-cities.md) — Fictional cloud-city districts and lift schedules. Base path `/v1/cloud-cities`
- [undersea-trains](docs/undersea-trains.md) — Fictional abyssal rail lines and station names. Base path `/v1/undersea-trains`
- [clockwork](docs/clockwork.md) — Fictional gear catalogs and winding intervals. Base path `/v1/clockwork`
- [goblin-market](docs/goblin-market.md) — Fictional stall listings and invented currencies. Base path `/v1/goblin-market`
- [fairy-rings](docs/fairy-rings.md) — Fictional ring coordinates and visiting hours. Base path `/v1/fairy-rings`
- [djinn-lamps](docs/djinn-lamps.md) — Fictional lamp inventory and wish-ticket stubs. Base path `/v1/djinn-lamps`
- [crystal-caves](docs/crystal-caves.md) — Fictional cavern maps and glow indexes. Base path `/v1/crystal-caves`
- [sand-ships](docs/sand-ships.md) — Fictional desert vessel logs. Base path `/v1/sand-ships`
- [paper-planes](docs/paper-planes.md) — Fictional folded-craft flight cards. Base path `/v1/paper-planes`
- [library-of-babel](docs/library-of-babel.md) — Fictional shelf addresses for invented books. Base path `/v1/library-of-babel`
- [mirror-worlds](docs/mirror-worlds.md) — Fictional reflection-realm directories. Base path `/v1/mirror-worlds`
- [shadow-markets](docs/shadow-markets.md) — Fictional night-bazaar booth names. Base path `/v1/shadow-markets`
- [comet-mail](docs/comet-mail.md) — Fictional message capsules on made-up comets. Base path `/v1/comet-mail`
- [asteroid-motels](docs/asteroid-motels.md) — Fictional roadside lodging on fictional rocks. Base path `/v1/asteroid-motels`
- [nebula-tea](docs/nebula-tea.md) — Fictional tea blends named after invented nebulae. Base path `/v1/nebula-tea`
- [robot-butlers](docs/robot-butlers.md) — Fictional household automaton nameplates. Base path `/v1/robot-butlers`
- [mech-hangars](docs/mech-hangars.md) — Fictional walker bay assignments. Base path `/v1/mech-hangars`
- [plasma-forges](docs/plasma-forges.md) — Fictional forge queue tickets. Base path `/v1/plasma-forges`
- [quantum-lockets](docs/quantum-lockets.md) — Fictional locket pairing codes. Base path `/v1/quantum-lockets`
- [echo-chambers](docs/echo-chambers.md) — Fictional acoustic room cards. Base path `/v1/echo-chambers`
- [lighthouse-ghosts](docs/lighthouse-ghosts.md) — Fictional keeper shift boards. Base path `/v1/lighthouse-ghosts`
- [map-shops](docs/map-shops.md) — Fictional chart sellers and blank-map SKUs. Base path `/v1/map-shops`
- [balloon-posts](docs/balloon-posts.md) — Fictional airmail balloon routes. Base path `/v1/balloon-posts`
- [ice-palaces](docs/ice-palaces.md) — Fictional wing names and thaw alarms. Base path `/v1/ice-palaces`
- [volcano-forges](docs/volcano-forges.md) — Fictional caldera workshop slips. Base path `/v1/volcano-forges`
- [star-charts](docs/star-charts.md) — Fictional constellation stickers. Base path `/v1/star-charts`
- [moon-rabbits](docs/moon-rabbits.md) — Fictional lunar hare census cards. Base path `/v1/moon-rabbits`
- [sunken-libraries](docs/sunken-libraries.md) — Fictional drowned-stack call numbers. Base path `/v1/sunken-libraries`
- [floating-markets](docs/floating-markets.md) — Fictional barge vendor lists. Base path `/v1/floating-markets`
- [gear-dragons](docs/gear-dragons.md) — Fictional mechanical wyrm serials. Base path `/v1/gear-dragons`
- [ink-spirits](docs/ink-spirits.md) — Fictional manuscript familiars. Base path `/v1/ink-spirits`
- [brass-birds](docs/brass-birds.md) — Fictional ornamental automaton flocks. Base path `/v1/brass-birds`
- [silk-roads-sky](docs/silk-roads-sky.md) — Fictional aerial caravan manifests. Base path `/v1/silk-roads-sky`
- [obsidian-gates](docs/obsidian-gates.md) — Fictional gatehouse visitor slips. Base path `/v1/obsidian-gates`
- [pearl-divers](docs/pearl-divers.md) — Fictional dive-bell shift cards. Base path `/v1/pearl-divers`
- [thunder-drums](docs/thunder-drums.md) — Fictional festival drum lineups. Base path `/v1/thunder-drums`
- [frost-gardens](docs/frost-gardens.md) — Fictional glasshouse bed labels. Base path `/v1/frost-gardens`
- [ember-foxes](docs/ember-foxes.md) — Fictional creature spotting cards. Base path `/v1/ember-foxes`
- [void-post](docs/void-post.md) — Fictional empty-space mailbox numbers. Base path `/v1/void-post`

## Fictional bestiary services

- [lantern-fish](docs/lantern-fish.md) — Fictional deep-lantern fish sighting cards. Base path `/v1/lantern-fish`
- [cloud-shepherds](docs/cloud-shepherds.md) — Fictional flock routes across invented skies. Base path `/v1/cloud-shepherds`
- [salt-wizards](docs/salt-wizards.md) — Fictional brine-guild membership slips. Base path `/v1/salt-wizards`
- [tea-oracles](docs/tea-oracles.md) — Fictional leaf-reading ticket stubs. Base path `/v1/tea-oracles`
- [bridge-trolls](docs/bridge-trolls.md) — Fictional toll-booth shift boards. Base path `/v1/bridge-trolls`
- [moon-bakeries](docs/moon-bakeries.md) — Fictional lunar pastry batch labels. Base path `/v1/moon-bakeries`
- [starlight-ink](docs/starlight-ink.md) — Fictional ink bottle lot numbers. Base path `/v1/starlight-ink`
- [wind-harps](docs/wind-harps.md) — Fictional harp tuning cards. Base path `/v1/wind-harps`
- [river-spirits](docs/river-spirits.md) — Fictional ford crossing permits. Base path `/v1/river-spirits`
- [glass-bees](docs/glass-bees.md) — Fictional hive window inventories. Base path `/v1/glass-bees`
- [copper-foxes](docs/copper-foxes.md) — Fictional den registry for story foxes. Base path `/v1/copper-foxes`
- [snow-giants](docs/snow-giants.md) — Fictional footprint measurement slips. Base path `/v1/snow-giants`
- [amber-flies](docs/amber-flies.md) — Fictional trapped-moment catalog. Base path `/v1/amber-flies`
- [velvet-bats](docs/velvet-bats.md) — Fictional roost assignment cards. Base path `/v1/velvet-bats`
- [iron-lilies](docs/iron-lilies.md) — Fictional garden plot tags. Base path `/v1/iron-lilies`
- [mist-ferries](docs/mist-ferries.md) — Fictional fog-route timetables. Base path `/v1/mist-ferries`
- [coral-choirs](docs/coral-choirs.md) — Fictional reef rehearsal schedules. Base path `/v1/coral-choirs`
- [quartz-owls](docs/quartz-owls.md) — Fictional night-watch roost lists. Base path `/v1/quartz-owls`
- [maple-drakes](docs/maple-drakes.md) — Fictional autumn wyrm census. Base path `/v1/maple-drakes`
- [pebble-golems](docs/pebble-golems.md) — Fictional stack-height permits. Base path `/v1/pebble-golems`
- [saffron-sails](docs/saffron-sails.md) — Fictional spice-ship manifests. Base path `/v1/saffron-sails`
- [indigo-whales](docs/indigo-whales.md) — Fictional song-catalog identifiers. Base path `/v1/indigo-whales`
- [cedar-dryads](docs/cedar-dryads.md) — Fictional grove tenancy cards. Base path `/v1/cedar-dryads`
- [tin-nightingales](docs/tin-nightingales.md) — Fictional music-box serials. Base path `/v1/tin-nightingales`
- [obsidian-moths](docs/obsidian-moths.md) — Fictional lamp-orbit logs. Base path `/v1/obsidian-moths`
- [pearl-moons](docs/pearl-moons.md) — Fictional satellite nickname registry. Base path `/v1/pearl-moons`
- [honey-comets](docs/honey-comets.md) — Fictional pastry-comet delivery slips. Base path `/v1/honey-comets`
- [basalt-turtles](docs/basalt-turtles.md) — Fictional island-shell mooring tags. Base path `/v1/basalt-turtles`
- [silver-minnows](docs/silver-minnows.md) — Fictional stream school counts. Base path `/v1/silver-minnows`
- [crimson-kites](docs/crimson-kites.md) — Fictional festival kite registrations. Base path `/v1/crimson-kites`
- [opal-snails](docs/opal-snails.md) — Fictional trail-map stickers. Base path `/v1/opal-snails`
- [azure-cranes](docs/azure-cranes.md) — Fictional migration postcard index. Base path `/v1/azure-cranes`
- [flint-sparrows](docs/flint-sparrows.md) — Fictional spark-nest inventories. Base path `/v1/flint-sparrows`
- [linen-ghosts](docs/linen-ghosts.md) — Fictional laundry-line haunting cards. Base path `/v1/linen-ghosts`
- [marble-seals](docs/marble-seals.md) — Fictional harbor stamp books. Base path `/v1/marble-seals`
- [willow-lamps](docs/willow-lamps.md) — Fictional riverside lamp routes. Base path `/v1/willow-lamps`
- [bronze-beetles](docs/bronze-beetles.md) — Fictional clock-beetle winding logs. Base path `/v1/bronze-beetles`
- [ivory-herons](docs/ivory-herons.md) — Fictional marsh lookout shifts. Base path `/v1/ivory-herons`
- [cinder-mice](docs/cinder-mice.md) — Fictional hearth census cards. Base path `/v1/cinder-mice`
- [gale-carp](docs/gale-carp.md) — Fictional wind-pond stocking slips. Base path `/v1/gale-carp`

## Crawl-friendly shards

Small files only. The bundled OpenAPI files are over GitHub's per-file index limit and are not extended here.

- Fictional ink-wyrm pen registry: docs/quill-wyrms.md and api/shards/quill-wyrms.json path /v1/quill-wyrms/search
- Fictional dock kelpie mooring slips: docs/harbor-kelpies.md and api/shards/harbor-kelpies.json path /v1/harbor-kelpies/search
- Fictional trunk-label prophecy cards: docs/attic-oracles.md and api/shards/attic-oracles.json path /v1/attic-oracles/search
- Fictional ember-thread batch tags: docs/cinder-loom.md and api/shards/cinder-loom.json path /v1/cinder-loom/search
- Fictional spore-line station names: docs/moss-telegraph.md and api/shards/moss-telegraph.json path /v1/moss-telegraph/search
- Fictional crystal-fruit plot numbers: docs/glass-orchard.md and api/shards/glass-orchard.json path /v1/glass-orchard/search
- Fictional salt-ledger page ids: docs/tide-scribes.md and api/shards/tide-scribes.json path /v1/tide-scribes/search
- Fictional ash-mail pouch numbers: docs/ember-post.md and api/shards/ember-post.json path /v1/ember-post/search
- Fictional ice-chapel bell schedules: docs/frost-bells.md and api/shards/frost-bells.json path /v1/frost-bells/search
- Fictional dye-moth lot cards: docs/saffron-moths.md and api/shards/saffron-moths.json path /v1/saffron-moths/search
- Fictional gutter-gauge readings: docs/copper-rain.md and api/shards/copper-rain.json path /v1/copper-rain/search
- Fictional night-pier berth slips: docs/velvet-docks.md and api/shards/velvet-docks.json path /v1/velvet-docks/search
- Fictional bone-white boat timetables: docs/ivory-ferries.md and api/shards/ivory-ferries.json path /v1/ivory-ferries/search
- Fictional black-glass loaf batches: docs/obsidian-bakery.md and api/shards/obsidian-bakery.json path /v1/obsidian-bakery/search
- Fictional lamp-card call numbers: docs/lantern-archive.md and api/shards/lantern-archive.json path /v1/lantern-archive/search
- Fictional barrel-hoop wind logs: docs/wind-cooper.md and api/shards/wind-cooper.json path /v1/wind-cooper/search
- Fictional oyster-line extension codes: docs/pearl-switchboard.md and api/shards/pearl-switchboard.json path /v1/pearl-switchboard/search
- Fictional hedge-mail route cards: docs/bramble-post.md and api/shards/bramble-post.json path /v1/bramble-post/search
- Fictional crystal-pantry shelf ids: docs/quartz-kitchen.md and api/shards/quartz-kitchen.json path /v1/quartz-kitchen/search
- Fictional leaf-flag semaphore cards: docs/maple-signal.md and api/shards/maple-signal.json path /v1/maple-signal/search
- Fictional blot-dock arrival slips: docs/inkwell-harbor.md and api/shards/inkwell-harbor.json path /v1/inkwell-harbor/search
- Fictional tree-shaft floor labels: docs/cedar-elevator.md and api/shards/cedar-elevator.json path /v1/cedar-elevator/search
- Fictional stitch-count job tickets: docs/silver-thimble.md and api/shards/silver-thimble.json path /v1/silver-thimble/search
- Fictional stone-stack call slips: docs/basalt-library.md and api/shards/basalt-library.json path /v1/basalt-library/search
- Fictional hive-line routing tags: docs/honey-switch.md and api/shards/honey-switch.json path /v1/honey-switch/search
- Fictional red-page manuscript ids: docs/crimson-folio.md and api/shards/crimson-folio.json path /v1/crimson-folio/search
- Fictional sky-clay firing tickets: docs/azure-kiln.md and api/shards/azure-kiln.json path /v1/azure-kiln/search
- Fictional spark-stall vendor cards: docs/flint-market.md and api/shards/flint-market.json path /v1/flint-market/search
- Fictional cloth-dome night logs: docs/linen-observatory.md and api/shards/linen-observatory.json path /v1/linen-observatory/search
- Fictional stone-bird cage numbers: docs/marble-aviary.md and api/shards/marble-aviary.json path /v1/marble-aviary/search
- Fictional riverside desk tickets: docs/willow-exchange.md and api/shards/willow-exchange.json path /v1/willow-exchange/search
- Fictional metal-fruit harvest slips: docs/bronze-orchard.md and api/shards/bronze-orchard.json path /v1/bronze-orchard/search
- Fictional shimmer-boat manifests: docs/opal-ferry.md and api/shards/opal-ferry.json path /v1/opal-ferry/search
- Fictional wind-folder call numbers: docs/gale-archive.md and api/shards/gale-archive.json path /v1/gale-archive/search
- Fictional ash-beam watch shifts: docs/cinder-lighthouse.md and api/shards/cinder-lighthouse.json path /v1/cinder-lighthouse/search
- Fictional brine-key tuning cards: docs/salt-piano.md and api/shards/salt-piano.json path /v1/salt-piano/search
- Fictional green-shaft floor names: docs/moss-elevator.md and api/shards/moss-elevator.json path /v1/moss-elevator/search
- Fictional pane-mail sorting slips: docs/glass-postmaster.md and api/shards/glass-postmaster.json path /v1/glass-postmaster/search
- Fictional wave-barrel lot tags: docs/tide-cooperage.md and api/shards/tide-cooperage.json path /v1/tide-cooperage/search
- Fictional coal-bird roost cards: docs/ember-aviary.md and api/shards/ember-aviary.json path /v1/ember-aviary/search

## Common pattern

```
GET /v1/{service}/{resource}
Accept: application/json
```

Query parameters used across the catalog: `q`, `limit`, `offset`, `lang`, `format`.

License: MIT.
