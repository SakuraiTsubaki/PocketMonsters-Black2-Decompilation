# Version Coverage

Use this document as the authoritative inventory of game versions targeted by this decompilation project.

The project has no local retail ROM baseline. Entries below therefore distinguish **release/product identity documented from public sources** from byte-level verification. A public catalogue hash or revision label is a research lead, not a project-level `Matched` result.

## Japanese baseline

| Status | Region / territory | Language | Revision / update | Product / build identifier | Release | Hashes | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Planned | Japan | Japanese | **Launch-retail revision unresolved.** Public preservation sources report a dumped `Rev 1` and list revision 0 as undumped. | `TWL-IREJ-JPN` / game code `IREJ` | 2012-06-23 | TBD | **Canonical survey baseline.** Nintendo/Pokémon official material confirms release date and product. Do not assume Rev 0 is the launch retail build; resolve cartridge revision evidence before assigning a baseline revision. |

## Regional / language targets

| Status | Region / territory | Language | Revision / update | Product / build identifier | Release | Hashes | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Planned | United States | English | TBD | `TWL-IREO-USA` / `IREO` | 2012-10-07 | TBD | North American launch date is independently documented; compare with EUR/AUS despite shared game code. |
| Planned | Australia | English | TBD | `TWL-IREO-AUS` / `IREO` | 2012-10-11 | TBD | Separate Australian retail identifier. |
| Planned | Europe | English | TBD | `TWL-IREO-EUR` / `IREO` | 2012-10-12 | Public reference: GameTDB CRC32 `185d037d`, MD5 `7496a685cb682ec8043a7a9aac1d187f`, SHA-1 `cea7defc3ee9c014c28cc04252fb2c25ef827cfb` | Nintendo Europe confirms 2012-10-12 launch. Public hash is not project-verified. |
| Planned | France / Europe | French | TBD | `TWL-IREF-FRA` / `IREF` | 2012-10-12 | Public reference: CRC32 `fc542c2e`, MD5 `f059c3868dadab1e48b930e361ca724e`, SHA-1 `3b6ed3120f10cf6fb3064d5d36dcc223156f8bd7` | Distinct French build identifier. |
| Planned | Germany / Europe | German | TBD | `TWL-IRED-NOE` / `IRED` | 2012-10-12 | TBD | Distinct German build identifier. |
| Planned | Italy / Europe | Italian | TBD | `TWL-IREI-ITA` / `IREI` | 2012-10-12 | TBD | Distinct Italian build identifier. |
| Planned | Spain / Europe | Spanish | TBD | `TWL-IRES-ESP` / `IRES` | 2012-10-12 | Public reference: CRC32 `67870079`, MD5 `ffa21be15d763fefc6b822a2be1fcf58`, SHA-1 `0779d08bb58c72512953bfb3593fb38beb17c669` | Distinct Spanish build identifier. |
| Planned | South Korea | Korean | Public catalogues report version 0; project verification pending | `TWL-IREK-KOR` / `IREK` | 2012-11-08 | Public reference: CRC32 `fc8335c5`, MD5 `5004816581dec88058807697637ed292`, SHA-1 `13dc1b9a8907387f82ee5a43462a07e7813860fd` | Korean launch independently documented; hashes from GameTDB remain public-reference evidence only. |
| Planned | Hong Kong | Japanese / TBD | TBD | TBD | 2012-06-23? | TBD | Secondary sources report same-day availability and Nintendo Hong Kong later lists the title as supported. Exact retail SKU/build relationship to Japan must be established. |
| Planned | Taiwan | Japanese / TBD | TBD | TBD | 2012-06-23? | TBD | Secondary sources report same-day availability. Determine whether this was Japanese software distribution rather than a distinct executable build. |
| Planned | Canada | English/French packaging | TBD | likely `IREO` family; exact retail suffix/build mapping TBD | 2012-10-07? | TBD | Dedicated packaging/build research required; do not collapse into US without evidence. |
| Planned | New Zealand | English / TBD | TBD | TBD | 2012-10-11? | TBD | Determine whether Australian build was distributed unchanged. |
| Planned | Singapore / other officially served Asian markets | English/Japanese / TBD | TBD | TBD | TBD | TBD | Research target; require primary or preservation evidence before defining a build. |

## Revision alert: Japanese Black 2

Public preservation material creates a non-trivial revision question:

- No-Intro's Japan undumped list records `IREJ` revision 0 as undumped and states that `Rev 1` was dumped before release date.
- GameHacking.org also indexes `Pocket Monsters - Black 2 (Japan) (Rev 1)`.

This does **not** by itself prove every launch retail cartridge was Rev 1. The baseline remains `TBD` until cartridge/header evidence and independent preservation metadata are reconciled.

## Current source anchors

- Nintendo Japan B2W2 page: https://www.nintendo.co.jp/ds/irej/index.html
- Pokémon official B2W2 product page: https://www.pokemon.co.jp/ex/b2w2/product/
- Nintendo corporate regional release table: https://www.nintendo.co.jp/ir/pdf/2013/130131.pdf
- Nintendo Europe launch notice: https://www.nintendo.com/en-gb/News/2012/Pokemon-Black-Version-2-Pokemon-White-Version-2-and-Pokemon-Dream-Radar-launching-October-12th-2012-647545.html
- GameFAQs release/product catalogue: https://gamefaqs.gamespot.com/ds/661226-pokemon-black-version-2/data
- No-Intro Japan undumped research: https://wiki.no-intro.org/index.php?title=Nintendo_-_Nintendo_DS%28i%29_Japan_undumped
- GameTDB English entry: https://www.gametdb.com/DS/IREO
- GameTDB Korean entry: https://www.gametdb.com/DS/IREK

## Status vocabulary

- **Planned** — target is in scope; identity may be partly documented, but project-level build verification is not complete.
- **Verified** — exact target identity and hashes have been independently confirmed under the repository verification rules.
- **Mapped** — executable/data layout documented for that exact target.
- **In progress** — active source reconstruction.
- **Matched** — reconstruction verified against the exact target using a defined matching criterion.
- **Reference only** — used for comparison but not a reconstruction target.

## Recording rules

1. The Japanese release is the starting comparison baseline, but its exact revision must be proven rather than assumed.
2. Record exact revision/update information whenever known; use `TBD` when it is not.
3. Prefer cryptographic hashes over filenames as identity evidence, but distinguish public-reference hashes from project-verified hashes.
4. Do not commit retail game images, decrypted game images, console keys, or ROM binaries.
5. Record regional, territory, packaging, language, and revision differences instead of assuming releases are identical.
6. If two territories share a game code, byte identity still requires verification.
7. Link version-specific findings to relevant documentation, manifests, or verification records.