# Public Source Survey — Pokémon Black 2

## Project premise

This reconstruction phase assumes **no local retail ROM is available**. Research must therefore be built from publicly accessible official material, technical documentation, source code, preservation records, archival material, and independently published reverse-engineering results.

No byte-level claim is treated as verified merely because it is commonly repeated. Findings that normally require direct ROM inspection remain explicitly unverified until corroborated by public technical evidence or multiple independent sources.

## Canonical survey axis: Japan first, all official regions compared

The original Japanese release is the starting comparison baseline. This is a survey baseline, not an assumption that the Japanese build is always the final or most-correct implementation.

Every officially released regional, territorial, language, packaging, and revision target discovered during research must be inventoried independently. Later revisions are separate records. "International" is not a substitute for enumerating actual builds.

For Black 2 specifically, the Japanese revision identity is already a research issue: public preservation sources report a dumped `IREJ Rev 1` while listing revision 0 as undumped. The launch-retail baseline revision must therefore remain unresolved until stronger evidence is reconciled.

## Evidence classes

- **Primary / official** — Nintendo, The Pokémon Company, Pokémon Korea, manuals, service notices, distribution notices, developer/publisher material.
- **Technical implementation** — public code or tools implementing Generation V formats or behavior.
- **Reverse engineering** — published analysis of executables, overlays, scripts, NARC paths, saves, file formats, or runtime behavior.
- **Preservation archive** — archived event files, C-Gear/Pokédex skins, PWT downloads, Dream World material, manuals, screenshots, web captures, catalogues, and metadata.
- **Secondary reference** — maintained databases and encyclopedias used for cross-checking releases, names, mechanics, locations, and differences.
- **Unverified report** — isolated claims that still require corroboration.

## Initial source inventory

### Official / first-party

- Nintendo Japan B2W2 page: https://www.nintendo.co.jp/ds/irej/index.html
- Pokémon official B2W2 site: https://www.pokemon.co.jp/ex/b2w2/
- Product information: https://www.pokemon.co.jp/ex/b2w2/product/
- Nintendo corporate regional launch table: https://www.nintendo.co.jp/ir/pdf/2013/130131.pdf
- Nintendo Europe 2012-10-12 launch notice: https://www.nintendo.com/en-gb/News/2012/Pokemon-Black-Version-2-Pokemon-White-Version-2-and-Pokemon-Dream-Radar-launching-October-12th-2012-647545.html
- Nintendo Hong Kong DS Wi-Fi service list: https://www.nintendo.com/hk/pressrelease/wifi_20140227.html

### Preservation / revision research

- No-Intro Nintendo DS(i) Japan undumped list: https://wiki.no-intro.org/index.php?title=Nintendo_-_Nintendo_DS%28i%29_Japan_undumped
- GameFAQs release/product catalogue: https://gamefaqs.gamespot.com/ds/661226-pokemon-black-version-2/data
- GameTDB English build metadata: https://www.gametdb.com/DS/IREO
- GameTDB Korean build metadata: https://www.gametdb.com/DS/IREK

### Generation V technical sources

- PKHeX: https://github.com/kwsch/PKHeX
- Project Pokémon Generation V research and event archive: https://projectpokemon.org/
- ndspy: https://github.com/RoadrunnerWMC/ndspy
- Tinke: https://github.com/pleonex/tinke
- TinkeDSi: https://github.com/R-YaTian/TinkeDSi
- AnimaEngine: https://github.com/KillDaWill/AnimaEngine
- The Cutting Room Floor: https://tcrf.net/

## Black 2-specific workstreams

1. Japanese launch baseline and exact revision identity (`IREJ`, Rev 0/Rev 1 question).
2. Complete regional/language/territory inventory and product-code map.
3. Japanese-baseline-to-region difference matrix.
4. ARM9/ARM7/overlay and NitroFS/NARC structure.
5. Scripts, events, flags, variables, maps, matrices, objects, warps, and encounters.
6. Pokémon, forms, personal data, moves, abilities, items, trainers, AI, and battle rules.
7. Text, encoding, fonts, UI, and localization differences.
8. Graphics, sprites, animation, models, palettes, UI, and audio.
9. Save structure, checksums, C-Gear, infrared, wireless, Wi-Fi, Entralink, Game Sync, PGL, and Dream World.
10. Mystery Gifts and regional distributions.
11. Pokémon World Tournament, Pokéstar Studios, Join Avenue, Hidden Grotto, Medal System, Memory Link, Key System, Funfest Missions, Black Tower, and difficulty modes.
12. Unused/dummy/debug content, bugs, revision fixes, and localization-specific corrections.
13. Structural continuity and differences versus Black/White and versus White 2.

## GitHub as authoritative project record

Research is not considered integrated merely because it appeared in chat. Findings, evidence, unresolved questions, manifests, tools, reconstructed data, and verification results must be committed to this repository (or explicitly linked to the relevant Generation V repository) to become part of the project record. Retail ROM binaries remain excluded.

## Research rule

The goal is not to copy a single wiki, database, or tool. Each subsystem should be reconstructed from multiple source classes where possible, and conflicts must be recorded rather than silently resolved.