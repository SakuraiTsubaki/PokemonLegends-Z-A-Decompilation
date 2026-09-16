# Target Profile: Pokémon Legends: Z-A

## Known repository scope

- Repository: `SakuraiTsubaki/PokemonLegends-Z-A-Decompilation`
- Working target name: Pokémon Legends: Z-A
- Platform family: Nintendo Switch / Nintendo Switch 2 Edition
- Series generation: Generation IX
- Exact release, region, revision, and build: **not yet selected**

The repository name is a working label, not proof of a particular binary. No address, symbol, format, or behavior should be treated as target fact until the exact build is identified.

## Identity checklist

Record all available items before substantive reconstruction:

- official title and product identifier;
- platform and execution environment;
- region, language, revision, update, and distribution form;
- hashes for user-supplied images, executables, modules, or manifests;
- executable/container layout and relevant segment identifiers;
- analysis, extraction, compiler, linker, and SDK tool versions;
- legal provenance and distribution constraints for every input;
- differences from related versions that affect addresses, formats, or behavior.

Store machine-readable identifiers in `config/target.json`. Store restricted inputs outside Git.

## Initial research priorities

- Identify the exact Nintendo Switch or Nintendo Switch 2 Edition, title update, distribution, and executable build IDs before analysis.
- Keep platform edition and update boundaries explicit; never transfer addresses, symbols, layouts, or verification results between builds without comparison.
- Inventory executable modules, relocations, runtime/SDK interfaces, RomFS layout, and edition-specific data boundaries.
- Document target-specific archives, serialization, compression, graphics, text, audio, area data, encounters, and scripts.
- Keep keys, firmware, packages, decrypted modules, and extracted content outside Git; build deterministic cross-edition and cross-version comparison tools.

## First milestone

The foundation milestone is complete when the exact target build is recorded, the initial file/executable map is reproducible, at least one research record has been promoted to an analysis with stated confidence, and all commands needed to repeat that result are documented.
