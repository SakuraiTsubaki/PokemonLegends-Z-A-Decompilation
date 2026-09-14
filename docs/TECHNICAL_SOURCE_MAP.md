# Technical Source Map

This document maps high-value public technical sources for Pokémon Legends: Z-A. It is a public-source reconstruction aid, not a substitute for direct target-build observation.

## Evidence boundary

The project currently has no local retail ROM/game dump. Findings below are public-source evidence from source code, documentation, datamines and reverse-engineering tools. They are not project `Observed` results until independently reproduced against an identified target.

## Save-data structure — PKHeX

Canonical source: `kwsch/PKHeX`.

PKHeX has a dedicated `SAV9ZA` save type and `SaveBlockAccessor9ZA`; it does not model Z-A as an SV save variant. Public source search currently exposes Z-A-specific structures including:

- party data (`Party9a`)
- trainer/status data (`MyStatus9a`)
- play time (`PlayTime9a`)
- box layout (`BoxLayout9a`)
- configuration (`ConfigSave9a`)
- Mable research progress (`MableStatus9a`)
- coordinates and map-name storage (`Coordinates9a`)
- player fashion (`PlayerFashion9a`)
- donut inventory/editor structures
- Infinite Royale state (`InfiniteRoyale9a`)
- stored shiny-entity handling

The dedicated accessor and substructure tree are strong public evidence that Z-A save layout must remain separate from Scarlet/Violet implementation details.

Public issue/release history can also reveal revision-specific layout changes, but issue reports are leads rather than authoritative observations and must be independently checked.

## FlatBuffers and hashes — PokeDocs

Canonical source: `pkZukan/PokeDocs`.

The dedicated `ZA/` tree contains both `Flatbuffers/` and `Hashlists/`. The current top-level FlatBuffers inventory includes:

- `dress_up_data.fbs`
- `event/`
- `scene/`
- `tracr.fbs`
- `trpmcatalog.fbs`

This differs materially from the much broader top-level category split in the SV PokeDocs tree. Do not force SV schemas onto Z-A.

Every file below `ZA/Flatbuffers/event`, `ZA/Flatbuffers/scene`, and `ZA/Hashlists` must be enumerated in later sweeps.

## Containers and resource formats

### `zbirow/Pokemon-Legends-Z-A-Tools`

Documents PFS0/NCA context and the Z-A TRPFS/TRPFD relationship. Its public documentation describes `data.trpfd` as a name/index source, `data.trpfs` as the main ONEPACK data store, FNV-1a name hashing and offset-based pack slicing.

### `pkZukan/gftool` / Trinity lineage

Although gftool documentation explicitly names earlier Trinity titles for some features, its serializers and related PokeDocs schemas are an important lineage source. Z-A-specific applicability must be verified per format rather than inherited automatically.

### Model/animation tooling

- `ChicoEevee/Pokemon-Switch-Model-Importer-Blender`
- `ChicoEevee/PokeModding-PLA-SV-Blender`
- `AncientDbri/Pokemon-Switch-Model-Importer-Plus`
- `KillzXGaming/Switch-Toolbox`

These provide leads for TRSKL/TRMSH/TRMBF, animations, textures and Trinity-related resources. Upstream/derivative relationships must be recorded to avoid treating copied support as independent research.

## Text and structured datamines

- `projectpokemon/za-textport` — multilingual JPN/Korean/English/French/German/Italian/Spanish/LATAM/Simplified/Traditional Chinese text plus Raw, Scrubbed Data and Trainers.
- `CPokemon/plza-text` — independent public Z-A text dump; compare coverage and hashes against `za-textport` before treating it as an independent data source.
- `Digote/pokedat` — `.dat`/`.tbl` text read/write/merge/split tooling with explicit LZA support.
- `Ruimusume/PLZA` — personal, Pokémon forms, item IDs, move IDs and donut-related structured data.
- `kwsch/pkNX` — public data-dumping/parsing lineage with explicit Z-A dumping support.
- `KotMatrosk1n/KM-Editor` — Z-A-specific public data models/editors spanning Pokémon, trainers, moves, items, encounters, placement, models and audio.

## Runtime/debug/mod research

- `Martmists-GH/switch-mods` — runtime/debug/Trinity-bypass leads.
- `borgox/Pokemon-Legends-Z-A-Mods` — aggregation of public mods/cheats and upstream links; useful for discovery only until each upstream source is verified.
- GBAtemp/other runtime-address threads — lead sources only; technical claims require independent verification.

## Next technical enumeration targets

Status remains **Sweeping**.

- enumerate all PKHeX `Gen9/ZA` save substructures and block keys
- enumerate `PokeDocs/ZA/Flatbuffers/event`, `scene`, and `Hashlists` file-by-file
- map Z-A quest/event, Wild Zone, Battle Zone, Z-A Royale, Infinite Royale, Mega Evolution, donut and Mega Dimension save/data structures
- distinguish base-game revision 1, Mega Dimension/2.0.x and later save/layout changes
- enumerate resource file extensions, hash lists, models, animation, textures, shaders, effects, audio and placement formats
- cross-compare `za-textport`, `plza-text`, `pokedat`, `PLZA`, pkNX and KM Editor to identify shared upstream data versus independent findings
