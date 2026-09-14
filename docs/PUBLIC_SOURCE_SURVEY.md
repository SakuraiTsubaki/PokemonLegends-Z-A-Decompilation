# Public Source Survey

This project currently has no local retail ROM/game dump. Reconstruction therefore begins with an exhaustive survey of publicly accessible evidence.

## Exhaustive means exhaustive

A category is not complete because one representative source was found. Every discoverable relevant page, repository, dataset, tool, archive, version, regional notice, language resource, event, distribution, and technical document must be enumerated or explicitly ruled out.

Japanese release/presentation is the comparison origin. This is a comparison axis, not an assumption that separate region-specific binaries exist.

## Required source families

| Family | Required coverage | Status |
| --- | --- | --- |
| Japanese official Pokémon/Nintendo | product pages, news archives, update notices, DLC, gifts, ranked battles, distributions, HOME, purchase bonuses | Sweeping |
| Korean official Pokémon/Nintendo | same categories, independently enumerated | Sweeping |
| North American official Pokémon/Nintendo | same categories, independently enumerated | Sweeping |
| European and other official regional sites | every available localization/region and date/wording difference | Sweeping |
| Pokémon HOME | compatibility, transfer rules, app update history, Research Tasks and title restrictions | Sweeping |
| GitHub reverse-engineering tools | parsers, editors, loaders, viewers, dumpers, hooks, debug tools, format libraries | Sweeping |
| GitHub datamines/datasets | multilingual text, personal data, forms, moves, items, encounters, trainers, placement, quests and DLC data | Sweeping |
| File-format research | PFS0/NCA context, TRPFS/TRPFD, Trinity, FlatBuffers, DAT/TBL text, models, animation, textures, shaders, audio, placement and hashes | Sweeping |
| Graphics/model resources | model/animation/import-export tooling and publicly referenced extracted resources; rights reviewed separately | Sweeping |
| Audio resources | banks, identifiers, cries, BGM, SFX, decoder/tool documentation | Sweeping |
| Maps/world | Lumiose City sectors, Wild Zones, Battle Zones, facilities, placement, encounter maps and DLC hyperspace areas | Sweeping |
| Mechanics | real-time battle, dodging, capture, Mega Evolution, Z-A Royale, online battle rules, movement and quest systems | Sweeping |
| Events/distributions | every Mystery Gift, serial/password distribution, ranked-battle Mega Stone reward, promotion and linked campaign | Sweeping |
| DLC | Mega Dimension purchase content, additional story, new Pokémon/forms, items, systems, patches and linked events | Sweeping |
| Secondary databases | Bulbapedia, Serebii, Pokémon Database and other structured references, used for discovery/cross-checking | Sweeping |
| Project Pokémon / specialist communities | research threads, datamines, tools, event archives and technical findings | Sweeping |
| Runtime/mod research | debug menus, Trinity bypasses, hooks, cheats and executable-address research; treated as leads until independently verified | Sweeping |
| Unused/deleted/debug material | documented unused data, leftovers, debug hooks/menus, placeholders and removed content | Sweeping |
| Historical/archived pages | retired official pages, old revisions, mirrors and web archives where legally/publicly accessible | Sweeping |

## Status vocabulary

- **Not started** — no systematic search yet.
- **Sweeping** — active broad search; results are incomplete.
- **Catalogued** — discovered sources are individually registered with provenance.
- **Cross-checked** — major claims have been compared against independent sources.
- **Exhausted** — multiple search strategies, languages, archives and source families have been searched with no remaining known uncatalogued leads. This status must not be used casually.

## Recording rule

Every result goes to GitHub. `manifests/public-source-catalog.csv` is the page/repository-level discovery catalog. `manifests/source-registry.json` contains higher-value source records and policy metadata. Detailed findings belong in `docs/`, structured reconstructed data in `data/`, tooling in `tools/`, and identity/provenance records in `manifests/`.

## Current sweep

The initial broad sweep has identified official Z-A news/update/HOME/DLC sources; pkNX; KM Editor; PokeDocs; Project Pokémon's multilingual `za-textport`; `pokedat`; Z-A TRPFS/TRPFD research tooling; structured PLZA personal/form/item/move data; Switch Pokémon model/animation tooling; runtime debug/Trinity bypass work; a public mod/cheat aggregation with upstream leads; and major secondary databases. This is a discovery baseline only and is explicitly **not exhaustive yet**.
