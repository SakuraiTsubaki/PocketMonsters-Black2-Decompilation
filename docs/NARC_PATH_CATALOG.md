# NARC / NitroFS Path Catalog — Pokémon Black 2

## Purpose

This document records publicly documented NitroFS/NARC paths for Pokémon Black 2 under the project's no-local-ROM policy. It separates archive existence/count evidence from semantic-role evidence and preserves source conflicts instead of silently choosing whichever old tool is convenient.

The machine-readable companion is `../manifests/narc-paths.csv`.

## Verification policy

- External tools/research do not automatically produce project-level `Observed` status.
- `Corroborated` means independent public technical sources agree.
- `Direct technical` means a public implementation or detailed format research directly targets the path.
- `Single-source` means one credible technical source currently supports the semantic role.
- Raw DB member counts are preservation metadata and remain unverified by this project.

## Initial path catalog

| Path | Reported role | Public member count | Evidence | Notes |
| --- | --- | ---: | --- | --- |
| `/a/0/0/2` | Main/system text | 495 | Direct technical | PPRE maps B2W2 main text here; Raw DB supplies count. |
| `/a/0/0/3` | Story text | 676 | Corroborated | PPRE + B2W2 General ROM Info; Raw DB count. |
| `/a/0/0/8` | Map resources | 1065 | Corroborated | B2W2 General ROM Info + independent ROM-content documentation; Raw DB count. |
| `/a/0/1/1` | Battle backgrounds | 572 | Direct technical | B2W2 General ROM Info; Raw DB count. |
| `/a/0/1/2` | ZoneData | 1 | Direct technical | B2W2 General ROM Info; Raw DB count. |
| `/a/0/1/6` | Pokémon personal data | 710 | Corroborated | B2W2 General ROM Info + PPRE; Raw DB count. |
| `/a/0/1/7` | Experience/growth table | 8 | Direct technical | PPRE + Raw DB count. |
| `/a/0/1/8` | Level-up learnsets | 709 | Corroborated | B2W2 General ROM Info + PPRE + Raw DB. |
| `/a/0/1/9` | Evolution data | 709 | Corroborated | B2W2 General ROM Info + PPRE + Raw DB. |
| `/a/0/2/0` | Base-evolution / baby-Pokémon lookup (legacy PPRE terminology) | 685 | Direct technical | PPRE role label; Raw DB count. Exact semantic structure still requires dedicated verification. |
| `/a/0/2/1` | Move data | 560 | Corroborated | B2W2 General ROM Info + PPRE + Raw DB. |
| `/a/0/2/4` | Item data | 639 | Direct technical | PPRE + Raw DB. |
| `/a/0/2/6` | Title-screen resources | 15 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/0/3/0` | Start-menu sprite/resources | 24 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/0/4/8` | Overworld sprites | 975 | Corroborated | Public B2W2 ROM-content documentation + Raw DB count. |
| `/a/0/5/6` | In-game scripts | 1289 | Corroborated | B2W2 General ROM Info; independent starter/script research confirms concrete script use; Raw DB count. |
| `/a/0/6/5` | Move animations | 601 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/0/7/1` | Animated trainer sprites (front / VS) | 1504 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/0/7/2` | Animated trainer sprites (back / send-out) | 248 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/0/9/1` | Trainer metadata (`trdata`) | 814 | Corroborated | B2W2 General ROM Info, TrainerTyrant, and Triple-Battle-Converter agree; Raw DB count. |
| `/a/0/9/2` | Trainer parties (`trpoke`) | 814 | Corroborated | B2W2 General ROM Info + TrainerTyrant; Raw DB count. |
| `/a/1/0/6` | Battle-facility/PWT banlist container | 38 | Single-source technical analysis | Public research documents facility/PWT banlist files in this NARC; Raw DB count. Exact file-level mapping will be split into a dedicated battle-facility document. |
| `/a/1/2/4` | Egg moves | 650 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/1/2/6` | Overworld/map-event data | 616 | Corroborated | B2W2 General ROM Info + independent hacking reports; Raw DB count. |
| `/a/1/2/7` | Wild encounter tables | 135 | Corroborated | B2W2 General ROM Info + independent wild-editing research; Raw DB count. |
| `/a/1/6/3` | In-game trades | 31 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/2/6/7` | Trainer mugshots | 76 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/2/7/3` | Hidden Grotto encounter table | 20 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/2/8/2` | Poké Mart data | 80 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/2/9/1` | PWT board trainer sprites | 472 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/a/2/9/6` | Pokédex in-game location data | 58 | Direct technical | B2W2 General ROM Info + Raw DB count. |
| `/skb.narc` | Role not yet assigned | 6 | Structural only | Raw DB confirms archive/count; do not infer semantic role from filename. |
| `/soundstatus.narc` | Role not yet assigned | 4 | Structural only | Raw DB confirms archive/count; semantic role TBD. |
| `/swan_sound_data.sdat` | Nintendo DS sound archive/container; internal mapping TBD | not NARC | Structural only | Raw DB records a non-NARC root sound archive. |

## Archive census baseline

Project Pokémon Raw DB enumerates **308 NARC entries** for its Pokémon Black 2 reference tree (link indices 0–307), plus explicitly non-NARC files. That census is not automatically the Japanese canonical baseline: the exact region/revision used by the Raw DB must be established first, especially because the Japanese `IREJ` launch-revision question is unresolved.

The complete census will be integrated incrementally without assigning meanings to unknown paths merely from filenames or archive sizes.

## Confirmed BW → B2W2 path movement

| Subsystem | Black / White | Black 2 / White 2 |
| --- | --- | --- |
| In-game scripts | `/a/0/5/7` | `/a/0/5/6` |
| Trainer metadata | `/a/0/9/2` | `/a/0/9/1` |
| Trainer parties | `/a/0/9/3` | `/a/0/9/2` |
| Overworld/events | `/a/1/2/5` | `/a/1/2/6` |
| Wild encounters | `/a/1/2/6` | `/a/1/2/7` |

This table is a concrete reason to keep BW and B2W2 as separate reconstruction targets rather than treating the sequels as a drop-in expanded data set.

## Source conflict: legacy PPRE B2W2 mappings

Legacy PPRE `nds/files.py` maps Black 2 trainer metadata/parties to `/a/0/9/2` and `/a/0/9/3`, and encounter data to `/a/1/2/6`. Later dedicated B2W2 research and tools disagree:

- TrainerTyrant: B2W2 `trdata=/a/0/9/1`, `trpoke=/a/0/9/2`.
- Triple-Battle-Converter: B2W2 trainer data `/a/0/9/1`, 814 entries.
- B2W2 General ROM Info: `/a/0/9/1` Trainer Data, `/a/0/9/2` Trainer Pokémon, `/a/1/2/6` Overworlds, `/a/1/2/7` Encounter Tables.
- Raw DB member counts line up with those later mappings: 814/814 trainer archives and 616/135 overworld/encounter archives.

For these paths, the repository uses the later corroborated B2W2 mapping and records PPRE as a historical implementation conflict.

## Source anchors

- Project Pokémon Black 2 Raw DB: https://projectpokemon.org/rawdb/black2/narc.php
- B2W2 General ROM Info: https://projectpokemon.org/home/forums/topic/22629-b2w2-general-rom-info/
- PPRE `nds/files.py`: https://github.com/projectpokemon/PPRE/blob/master/nds/files.py
- PPRE `pokeversion.py`: https://github.com/projectpokemon/PPRE/blob/master/pokeversion.py
- TrainerTyrant: https://github.com/ThirdLemon/TrainerTyrant
- Triple-Battle-Converter: https://github.com/mFireworks/Triple-Battle-Converter
- B2W2 script/starter research: https://projectpokemon.org/home/forums/topic/13490-twistedfatal-black-and-white-toolbox/page/15/
- ROM-content cross-reference: https://whackahack.com/foro/threads/guia-nds-informacion-sobre-el-contenido-de-cada-rom-proceso.32504/

## Next work

1. Identify the exact region/revision represented by the Black 2 Raw DB tree.
2. Import the complete 308-entry archive census with unknown roles preserved as unknown.
3. Split personal, trainer, encounter, script, map/ZoneData, graphics, PWT, Hidden Grotto, shop, and audio formats into dedicated documents as evidence is collected.
4. Record file-level indices and structures (not only NARC paths) with source and confidence.
5. Compare Japanese `IREJ` against every regional build and against White 2 rather than assuming pair identity.