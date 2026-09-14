# Project Status

**Current stage:** Public-source survey and reconstruction baseline

This project currently assumes no local retail ROM baseline is available. Work therefore starts from public official material, preservation metadata, technical implementations, reverse-engineering research, and independently published evidence.

## Current baseline policy

- Japanese retail release is the canonical starting point for comparison.
- Every official regional/language/territory/revision target is tracked independently.
- Black 2 is not merged with White 2, Black, or White.
- Unknown fields remain `TBD`/`Unknown`; no revision, hash, offset, or build identity is invented.
- Public hashes and catalogue metadata are reference evidence until independently verified under `VERIFICATION.md`.
- Research is integrated only when committed to GitHub; retail ROM binaries remain excluded.

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

## Reconstruction progress

- [x] Repository policy, asset workflow, verification rules, and long-term structure established.
- [x] Public-source survey policy added.
- [x] Regional survey matrix added.
- [ ] Document executable and section layout.
- [ ] Map ARM9, ARM7, overlays, NitroFS, and NARC structure.
- [ ] Map symbols, functions, and major subsystems.
- [ ] Document game-data formats and resource containers.
- [ ] Reconstruct scripts, events, and behavior.
- [ ] Reconstruct asset pipelines and metadata.
- [ ] Document B2W2-specific systems (PWT, Pokéstar Studios, Join Avenue, Hidden Grotto, Medal, Memory Link, Key System, Funfest Missions, Black Tower, difficulty modes).
- [ ] Add reproducible extraction/repacking tooling from lawful user-provided inputs where required.
- [ ] Add automated verification where practical.

## Verification levels

- **Unverified** — proposed/imported claim not independently checked.
- **Observed** — confirmed directly in a specific target build, executable, extracted file, or runtime observation.
- **Reproduced** — recreated using documented steps, tooling, inputs, and target information.
- **Matched** — reconstructed output satisfies a defined exact-match criterion.

Because no local target ROM is currently available, most build-byte claims remain below `Observed` unless direct public technical evidence supports them.

## Next milestones

1. Resolve Japanese `IREJ` launch revision identity.
2. Finish regional/territory/product-code inventory and revision enumeration.
3. Build the first evidence-backed Nintendo DS/DSi executable and NitroFS/NARC map from public technical sources.
4. Start Japanese-baseline-to-region difference records with text/encoding/font and executable/resource distinctions kept separate.
5. Keep `VERSIONS.md`, `REGIONAL_SURVEY_MATRIX.md`, manifests, and verification records synchronized as evidence improves.