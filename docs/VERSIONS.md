# Version Coverage

Use this document as the authoritative inventory of game versions targeted by this decompilation project.

## Research baseline

The project currently has no local retail ROM, decrypted game image, or complete game dump. Version coverage therefore begins from public-source evidence. Japanese release / Japanese-language material is the origin reference for comparison, but this does not imply that Japan necessarily uses a distinct binary or package-internal data set.

## Initial official-source baseline

- **Title:** Pokémon Legends: Z-A
- **Original release date:** 2025-10-16
- **Platforms:** Nintendo Switch and Pokémon Legends: Z-A – Nintendo Switch 2 Edition
- **Latest software update confirmed in this baseline:** Ver. 2.0.2
- **US support release date for Ver. 2.0.2:** 2026-03-18
- **Officially listed languages:** Japanese, American English, French, Canadian French, German, Italian, Spanish, Latin American Spanish, Korean, Simplified Chinese, Traditional Chinese
- **DLC family:** Pokémon Legends: Z-A – Mega Dimension; Holo-X and Holo-Y Apparel Items; additional story content

These facts are public-source baseline facts, not hash-verified target identities.

## Language / regional comparison inventory

| Status | Baseline role | Region / distribution mapping | Language | Revision / update | Platform / build | Hashes | Evidence | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Planned | Origin reference | Japan reference | Japanese | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Starting comparison point; package/build identity still to be mapped |
| Planned | Compare to JP | TBD | American English | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | French | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | Canadian French | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | German | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | Italian | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | Spanish | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | Latin American Spanish | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | Korean | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | Simplified Chinese | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |
| Planned | Compare to JP | TBD | Traditional Chinese | Launch through Ver. 2.0.2 | Switch / Switch 2 Edition | unavailable | Official primary | Officially supported language |

## Update / DLC milestones currently seeded

| Date | Version / content | Scope | Evidence state | Notes |
| --- | --- | --- | --- | --- |
| 2025-10-16 | Launch / Ver. 1.0.1 update data available | Base game / online data | Official primary | Launch date; Nintendo update history lists Ver. 1.0.1 |
| 2025-11-05 (US) | Ver. 1.0.2 | Update | Official primary | Fixes and Ranked Battle balance adjustments |
| 2025-11-26 (US) | Ver. 1.0.3 | Update | Official primary | Ranked Battle reward issue fix |
| 2025-12-09 (US) | Ver. 2.0.0 | Update / DLC | Official primary | Mega Dimension additional story support and added Pokémon |
| 2026-01-21 (US) | Ver. 2.0.1 | Update | Official primary | DLC-related fixes and item adjustments |
| 2026-03-18 (US) | Ver. 2.0.2 | Update | Official primary | Latest update currently found; several issues fixed |

Regional support pages may display the following calendar day for the same rollout because of local time zones. Preserve those dates per source rather than flattening them into one universal date.

## Primary sources seeded in Phase 0

- Nintendo US Pokémon Legends: Z-A product page: https://www.nintendo.com/us/store/products/pokemon-legends-z-a-switch/
- Nintendo US Pokémon Legends: Z-A update history: https://en-americas-support.nintendo.com/app/answers/detail/a_id/68626
- Official Pokémon Legends: Z-A release announcement: https://legends.pokemon.com/en-us/news/release-date
- Official Mega Dimension information: https://legends.pokemon.com/en-us/dlc

## Status vocabulary

- **Planned** — intended for investigation but not yet directly verified against a target build.
- **Verified** — identity and hashes confirmed.
- **Mapped** — executable/data layout documented.
- **In progress** — active source reconstruction.
- **Matched** — reconstruction verified against the target.
- **Reference only** — used for comparison but not a reconstruction target.

## Recording rules

1. Record exact revision/update information whenever known.
2. Prefer cryptographic hashes over filenames as identity evidence.
3. Do not commit retail game images or console keys.
4. Record regional or language differences instead of assuming two releases are identical.
5. Start comparisons from the Japanese reference baseline, then enumerate every official language and distribution region discovered.
6. Keep Nintendo Switch and Nintendo Switch 2 Edition identity/build questions separate until evidence establishes what is shared and what differs.
7. Treat storefront/package region, language resources, executable identity, event availability, and service behavior as separate comparison axes.
8. Preserve local-date differences in official regional update notices rather than normalizing them away without explanation.
9. Link version-specific findings to relevant documentation, manifests, sources, or verification issues.