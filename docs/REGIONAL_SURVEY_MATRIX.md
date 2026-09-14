# Regional Survey Matrix — Pokémon Black 2

## Purpose

Track every officially released regional, territorial, language, packaging, and revision target of Pokémon Black 2 against the original Japanese release baseline.

The matrix is evidence-first. Use `Unknown` or `TBD` when a field has not been verified.

## Baseline policy

- Baseline axis: original Japanese retail release.
- The exact Japanese launch revision is currently unresolved.
- Every non-Japanese build is compared directly against the Japanese baseline once that baseline revision is established.
- Non-Japanese builds are also cross-compared where necessary.
- Revisions are separate records.
- Language, territory, cartridge identity, release date, revision, packaging, and technical differences must not be conflated.

## Build inventory

| Record ID | Version | Territory / market | Language | Release date | Revision | Product / cart code | Known hashes | Evidence status | Sources |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BLACK2-JP-BASE | Black 2 | Japan | Japanese | 2012-06-23 | **TBD — Rev 0/Rev 1 launch-baseline question** | `TWL-IREJ-JPN` / `IREJ` | TBD | Official release confirmed; revision unresolved | Nintendo JP; Pokémon official; No-Intro preservation research |
| BLACK2-US-EN | Black 2 | United States | English | 2012-10-07 | Unknown | `TWL-IREO-USA` / `IREO` | Unknown | Product/release catalogued | Nintendo regional release data; GameFAQs |
| BLACK2-AU-EN | Black 2 | Australia | English | 2012-10-11 | Unknown | `TWL-IREO-AUS` / `IREO` | Unknown | Product/release catalogued | GameFAQs |
| BLACK2-EU-EN | Black 2 | Europe | English | 2012-10-12 | Unknown | `TWL-IREO-EUR` / `IREO` | Public reference: CRC32 `185d037d`; MD5 `7496a685cb682ec8043a7a9aac1d187f`; SHA-1 `cea7defc3ee9c014c28cc04252fb2c25ef827cfb` | Release/product identity corroborated; bytes not project-verified | Nintendo Europe; GameFAQs; GameTDB |
| BLACK2-EU-FR | Black 2 | France / Europe | French | 2012-10-12 | Unknown | `TWL-IREF-FRA` / `IREF` | Public reference: CRC32 `fc542c2e`; MD5 `f059c3868dadab1e48b930e361ca724e`; SHA-1 `3b6ed3120f10cf6fb3064d5d36dcc223156f8bd7` | Product/release catalogued | GameFAQs; GameTDB |
| BLACK2-EU-DE | Black 2 | Germany / Europe | German | 2012-10-12 | Unknown | `TWL-IRED-NOE` / `IRED` | Unknown | Product/release catalogued | GameFAQs; GameTDB |
| BLACK2-EU-IT | Black 2 | Italy / Europe | Italian | 2012-10-12 | Unknown | `TWL-IREI-ITA` / `IREI` | Unknown | Product/release catalogued | GameFAQs; technical catalogue records |
| BLACK2-EU-ES | Black 2 | Spain / Europe | Spanish | 2012-10-12 | Unknown | `TWL-IRES-ESP` / `IRES` | Public reference: CRC32 `67870079`; MD5 `ffa21be15d763fefc6b822a2be1fcf58`; SHA-1 `0779d08bb58c72512953bfb3593fb38beb17c669` | Product/release catalogued | GameFAQs; GameTDB |
| BLACK2-KR | Black 2 | South Korea | Korean | 2012-11-08 | Public catalogue: v0; project verification pending | `TWL-IREK-KOR` / `IREK` | Public reference: CRC32 `fc8335c5`; MD5 `5004816581dec88058807697637ed292`; SHA-1 `13dc1b9a8907387f82ee5a43462a07e7813860fd` | Product/release corroborated; bytes not project-verified | Korean launch coverage; GameFAQs; GameTDB |
| BLACK2-HK | Black 2 | Hong Kong | Japanese / TBD | 2012-06-23? | Unknown | Unknown | Unknown | Official territory support later confirmed; exact retail build unresolved | Nintendo Hong Kong; secondary release records |
| BLACK2-TW | Black 2 | Taiwan | Japanese / TBD | 2012-06-23? | Unknown | Unknown | Unknown | Research target | Secondary release records; primary evidence pending |
| BLACK2-CA | Black 2 | Canada | English/French packaging | 2012-10-07? | Unknown | `IREO` family / exact retail suffix TBD | Unknown | Research target | Packaging/build evidence pending |
| BLACK2-NZ | Black 2 | New Zealand | English / TBD | 2012-10-11? | Unknown | Unknown | Unknown | Research target | Primary/preservation evidence pending |
| BLACK2-SG | Black 2 | Singapore / officially served Asian markets | English/Japanese / TBD | Unknown | Unknown | Unknown | Unknown | Research target | Primary/preservation evidence pending |

## Revision alert

Public preservation evidence requires special handling:

- No-Intro lists `IREJ` revision 0 as undumped and notes a dumped `Rev 1` before release date.
- Other public catalogues index `Pocket Monsters - Black 2 (Japan) (Rev 1)`.

Do not convert this into the claim "launch retail = Rev 1" until cartridge/header evidence and independent metadata are reconciled.

## Difference matrix

| Build ID | Category | Japanese baseline state | Regional state | Difference class | Evidence level | Source(s) | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| BLACK2-EU-FR / DE / IT / ES | language/build identity | Japanese `IREJ` | Distinct language game codes (`IREF`, `IRED`, `IREI`, `IRES`) | text / localization / encoding; potentially other technical differences | Corroborated for product identity; technical diff pending | GameFAQs; GameTDB; preservation catalogues | Separate build targets must be retained independently. |
| BLACK2-KR | language/build identity | Japanese `IREJ` | Korean `IREK` | text / localization / encoding; fonts/glyphs; potentially other technical differences | Corroborated for product identity; technical diff pending | GameFAQs; GameTDB | Korean target is first-class, not a generic international variant. |
| BLACK2-US-EN / EU-EN / AU-EN | territory/build identity | Japanese `IREJ` | Shared `IREO` game-code family with different retail suffixes | unclassified until byte-comparison evidence exists | Corroborated for retail identity | Nintendo/secondary catalogues | Shared game code does not prove byte identity. |

## Difference classes

- executable / ARM9 / ARM7
- overlay
- filesystem / NitroFS
- NARC membership / ordering / format
- Pokémon / personal data / forms
- moves / abilities / items
- encounters
- trainers / AI / battle rules
- maps / matrices / warps / objects
- scripts / flags / variables / events
- text / localization / encoding
- fonts / glyphs
- graphics / sprites / UI / models
- audio / music / SFX
- save structure / checksums
- wireless / infrared / Wi-Fi
- C-Gear / Entralink / Game Sync / Global Link
- Mystery Gift / external distribution
- PWT / Pokéstar Studios / Join Avenue / Hidden Grotto / Medal / Memory Link / Key System / Funfest / Black Tower
- unused / dummy / debug content
- bug / glitch / revision fix
- legal / ratings / censorship / localization adaptation
- packaging / manual / non-ROM material
- unclassified

## Evidence levels

- **Official** — official first-party material directly supports the claim.
- **Direct technical** — public code, extracted data, disassembly, or format implementation directly demonstrates the claim.
- **Corroborated** — two or more independent reliable sources agree.
- **Single-source** — one credible source exists but independent confirmation is pending.
- **Reported** — claim exists but technical verification is insufficient.
- **Unknown** — no adequate evidence yet.

## Source anchors

- https://www.nintendo.co.jp/ds/irej/index.html
- https://www.pokemon.co.jp/ex/b2w2/product/
- https://www.nintendo.co.jp/ir/pdf/2013/130131.pdf
- https://www.nintendo.com/en-gb/News/2012/Pokemon-Black-Version-2-Pokemon-White-Version-2-and-Pokemon-Dream-Radar-launching-October-12th-2012-647545.html
- https://gamefaqs.gamespot.com/ds/661226-pokemon-black-version-2/data
- https://wiki.no-intro.org/index.php?title=Nintendo_-_Nintendo_DS%28i%29_Japan_undumped
- https://www.gametdb.com/DS/IREO
- https://www.gametdb.com/DS/IREK

## Comparison rule

A localized text difference is not automatically a complete technical-ROM difference description. Record localization, then separately record any encoding, font, archive-layout, script, executable, or resource change.

A revision-specific bug fix must remain tied to the exact target until evidence shows it applies more broadly.