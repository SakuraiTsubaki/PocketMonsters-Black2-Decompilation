# Project Status

**Current stage:** Exhaustive public-source census and reconstruction baseline

This project assumes no local retail ROM baseline is available. Work therefore starts from public official material, preservation metadata, technical implementations, reverse-engineering research, historical web captures, and independently published evidence.

## Current baseline policy

- Japanese retail release is the canonical starting point for comparison.
- Every official regional/language/territory/revision target is tracked independently.
- Black 2 is not merged with White 2, Black, or White.
- Unknown fields remain `TBD`/`Unknown`; no revision, hash, offset, or build identity is invented.
- Public hashes and catalogue metadata are reference evidence until independently verified under `VERIFICATION.md`.
- Research is integrated only when committed to GitHub; retail ROM binaries remain excluded.
- **Subsystem reconstruction never replaces the exhaustive public-source census. Registered source classes remain open until their relevant child pages/files/releases/records are enumerated or explicitly documented as unavailable/blocked.**

## Source-census priority

- [x] Create exhaustive source-class registry (`docs/SOURCE_REGISTRY.md`).
- [x] Add machine-readable source inventory (`manifests/source-registry.csv`).
- [x] Register official JP/KR/US/EU/AU roots, manuals and online-service history.
- [x] Register preservation roots for Gen V events, Dream World, C-Gear, Pokédex skins, Musicals, PWT and server-format DLC.
- [x] Register major public Gen V code/tools and Nintendo DS format infrastructure.
- [x] Register unused/prerelease, secondary-reference, catalog/revision, physical-scan, guide, magazine, soundtrack and bug-research classes.
- [ ] Enumerate every relevant child page/file/release/record under every registered source root.
- [ ] Enumerate Internet Archive/Wayback captures for dead official, PGL, Dream World and regional sites.
- [ ] Enumerate every official event/distribution/service notice by region and language.
- [ ] Enumerate historical Gen V tools/research whose original hosting disappeared.
- [ ] Resolve blocked TCRF material through indexed/archived evidence without inventing inaccessible content.
- [ ] Do not mark `all public sources surveyed` while any mandatory class remains `Enumerating`, `Candidate`, `Blocked`, or otherwise unresolved.

## Version inventory status

- [x] Japanese product identity and official launch date documented (`IREJ`, 2012-06-23).
- [x] Major US/Australia/Europe/Korea product-code targets seeded.
- [x] Separate European English/French/German/Italian/Spanish targets recorded.
- [x] Hong Kong/Taiwan/Canada/New Zealand/other served-market questions added as explicit research targets.
- [x] Japanese Rev 0 / Rev 1 ambiguity recorded instead of assumed away.
- [ ] Resolve exact Japanese launch-retail revision with independent cartridge/header evidence.
- [ ] Enumerate every revision for every regional build.
- [ ] Independently verify public-reference hashes.
- [ ] Complete territory/packaging variants and official distribution channels.

## Technical reconstruction progress

- [x] Repository policy, asset workflow, verification rules, and long-term structure established.
- [x] Public-source survey policy and regional survey matrix added.
- [x] Evidence-backed NARC/NitroFS path catalog and machine-readable inventory added.
- [x] Record BW → B2W2 path relocation for scripts, trainers, overworlds, and encounters.
- [x] Preserve the legacy PPRE B2W2 trainer/encounter mapping conflict instead of silently inheriting it.
- [x] Record B2W2-specific path leads for ZoneData, egg moves, PWT, Hidden Grotto, shops, trades, trainer graphics, and move animations.
- [ ] Identify the exact region/revision represented by the public Black 2 Raw DB tree.
- [ ] Import the complete Raw DB archive census while preserving unknown roles.
- [ ] Resolve Japanese launch revision before treating any archive census as canonical Japan baseline.
- [ ] Document executable/section layout, ARM9/ARM7/overlays, symbols/functions, formats, scripts/events, asset pipelines, save/communication/online/distribution structures, unused/debug material and bugs.
- [ ] Fully document B2W2-specific systems (PWT, Pokéstar Studios, Join Avenue, Hidden Grotto, Medal, Memory Link, Key System, Funfest Missions, Black Tower, difficulty modes).
- [ ] Add reproducible tooling and automated verification where practical.

## Current technical baseline

Project Pokémon's Black 2 Raw DB publicly enumerates 308 NARC entries plus non-NARC root files. B2W2-specific research identifies numerous subsystem paths, and independent trainer tooling corroborates the trainer relocation to `/a/0/9/1` + `/a/0/9/2`. Encounter research places wild encounters at `/a/1/2/7` while `/a/1/2/6` is overworld/event data.

These findings remain public-source reconstruction evidence, not direct observation of a project-owned Japanese target ROM.

## Verification levels

- **Unverified** — a proposed/imported claim not independently checked against a project target.
- **Observed** — confirmed directly in a specific target build, executable, extracted file, or runtime observation.
- **Reproduced** — recreated using documented steps, tooling, inputs, and target information.
- **Matched** — reconstructed output satisfies a defined exact-match criterion.

Research documents may additionally mark evidence as corroborated, direct technical, single-source, structural-only, preserved, or conflicted without promoting project-level verification.

## Next milestones

1. Enumerate the registered public-source universe source-by-source and file/page-by-file/page before narrowing the project to any one subsystem.
2. Expand Japanese official sources first, then every regional/language official and archival branch.
3. Enumerate preservation/event/DLC collections and public code repositories at item/file level.
4. Resolve Japanese `IREJ` launch revision identity and identify the Raw DB source build in parallel without treating those tasks as the whole survey.
5. Keep `SOURCE_REGISTRY.md`, source manifest, `VERSIONS.md`, regional matrix, NARC catalog and this status synchronized.
