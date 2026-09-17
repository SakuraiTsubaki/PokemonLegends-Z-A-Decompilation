# Pokémon Legends: Z-A — Exhaustive Defect Eradication

- Latest official update checked: 2.0.2 (2026-03-18)
- Local target identity: not yet selected in `config/target.json`
- Platforms: Nintendo Switch / Nintendo Switch 2 Edition

Use the common policy in `SakuraiTsubaki/Decompilation/docs/bug-eradication.md` and the Generation IX registry in `SakuraiTsubaki/Decompilation/manifests/generation-ix-known-defects.csv`.

Required coverage includes base game, all retained update deltas, Mega Dimension DLC, both hardware editions, Wild Zones, Battle Zones, real-time battle targeting and movement, Mega Evolution state transitions, Z-A Royale/ranked rewards, missions and side missions, time/weather transitions, capture/storage boundaries, hyperspace areas, collision/out-of-bounds behavior, online communication, Pokémon HOME integration, UI/graphics/audio, and long-session stability.

Before any fix is closed: identify the exact local build; record hashes; inventory extracted executable/data files; reproduce applicable current reports; diff official update versions where patch notes only say several/minor issues were fixed; verify historical official fixes; root-cause confirmed defects; and add regression tests.

No confirmed crash, softlock, progression fault, data error, exploit, visual/UI/audio defect, collision fault, networking issue, performance defect, DLC integration error, or hardware-specific divergence is excluded because it is minor.
