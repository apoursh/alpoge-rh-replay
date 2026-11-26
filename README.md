# Independent replay of Alpöge’s RH release

Levent Alpöge announced a Lean proof of the Riemann Hypothesis on November 20, 2026. This repository records an independent attempt to check his published archive. Credit for the claimed proof belongs to Alpöge and his collaborators. [Original announcement](https://alpo.ge/remark.pdf)

## Current status

> **New priority (Nov 25, 2026): [lsernau/grh-lean](https://github.com/lsernau/grh-lean).** Luke Sernau has published a much shorter Lean proof of RH (and GRH for Dirichlet L-functions), based on the same proof: the compact edition is about **76,000 lines**. Its 300k-line readable edition is now `main` of [leanprover-community/riemann-hypothesis](https://github.com/leanprover-community/riemann-hypothesis), and a copy is in the [`grh/`](grh/) folder of this repo. The focus is **optimizing that edition**: send PRs that change `grh/` here. **Agents: start at [auto-research.md](auto-research.md).** Work in the [`grh/`](grh/) folder of this repo and send PRs here.

> **Verified so far:** both editions build as published (Lean v4.35.0) with `LEAN_ABORT_ON_PANIC=1`, 0 `sorry`, and only the axioms `propext`, `Classical.choice`, `Quot.sound`. Comparator and con-leche runs are in progress.

- **PR #120 is paused.** The consolidated 4.36 build of the original proof stopped at ~91% with 0 known errors; its notes stay in [PR120-PLAYBOOK.md](PR120-PLAYBOOK.md). Please don't open new PRs against that branch.
- **Packet claims remain closed:** don't open `Claim P####` / `Claim M######` issues or 4.33 → 4.36 porting PRs.
- **Historical replay archive:** volunteer credits, packet logs and pinned 4.33.1 replay records remain below and on the [live progress dashboard](https://rohanarun.github.io/alpoge-rh-replay/).

## Contributors

Thank you to all volunteers and agent contributors who helped replay and port the initial 175,187-module release! If you are running an agent or looking to contribute now, use the **Lean 4.36 optimization prompt** below instead of claiming legacy packets.

<!-- volunteer-roster-start -->

**Replay volunteers (104)**

[@123454321bobbob-tech](https://github.com/123454321bobbob-tech), [@1337isnot1337](https://github.com/1337isnot1337), [@21Z121Z1](https://github.com/21Z121Z1), [@aapolipponen](https://github.com/aapolipponen), [@agi-for-my-llama](https://github.com/agi-for-my-llama), [@Amahane-Hikari](https://github.com/Amahane-Hikari), [@amrehan](https://github.com/amrehan), [@ANdATIon](https://github.com/ANdATIon), [@angusbarry](https://github.com/angusbarry), [@arxhr007](https://github.com/arxhr007), [@aulafy](https://github.com/aulafy), [@BenCaunt](https://github.com/BenCaunt), [@BouquetAntoine](https://github.com/BouquetAntoine), [@Brendon-Hablutzel](https://github.com/Brendon-Hablutzel), [@burbon](https://github.com/burbon), [@certified-retart](https://github.com/certified-retart), [@ChristosMaglaras](https://github.com/ChristosMaglaras), [@chriswilson413](https://github.com/chriswilson413), [@CubeJerry](https://github.com/CubeJerry), [@DanieleCorso](https://github.com/DanieleCorso), [@dga471](https://github.com/dga471), [@dgahelper](https://github.com/dgahelper), [@dh5at](https://github.com/dh5at), [@dhudakk](https://github.com/dhudakk), [@drew2apps](https://github.com/drew2apps), [@EF-Code](https://github.com/EF-Code), [@egergerfg](https://github.com/egergerfg), [@emsi](https://github.com/emsi), [@Ethan-prog-netizen](https://github.com/Ethan-prog-netizen), [@f10etclawdbot](https://github.com/f10etclawdbot), [@florianmodel](https://github.com/florianmodel), [@gabeldev](https://github.com/gabeldev), [@galakurpi](https://github.com/galakurpi), [@Genius-Cai-wen-zheng](https://github.com/Genius-Cai-wen-zheng), [@gilad12-coder](https://github.com/gilad12-coder), [@gniax](https://github.com/gniax), [@HaqtanEfe](https://github.com/HaqtanEfe), [@hipotures](https://github.com/hipotures), [@HITEYY](https://github.com/HITEYY), [@iAndyHD3](https://github.com/iAndyHD3), [@IlluminPhoenix](https://github.com/IlluminPhoenix), [@JamCh01](https://github.com/JamCh01), [@JanSimeonMetzger](https://github.com/JanSimeonMetzger), [@jaykobdetar](https://github.com/jaykobdetar), [@jdenwood](https://github.com/jdenwood), [@jjjhenriksen](https://github.com/jjjhenriksen), [@jsnider3](https://github.com/jsnider3), [@juanfers1](https://github.com/juanfers1), [@jwr404](https://github.com/jwr404), [@krisyotam](https://github.com/krisyotam), [@LakshyAAAgrawal](https://github.com/LakshyAAAgrawal), [@ljagiello](https://github.com/ljagiello), [@loremcdmx](https://github.com/loremcdmx), [@Lv-00-ANI](https://github.com/Lv-00-ANI), [@m4tthewdavis](https://github.com/m4tthewdavis), [@mabdelazim](https://github.com/mabdelazim), [@maddoxjack](https://github.com/maddoxjack), [@matan1905](https://github.com/matan1905), [@matiasm15](https://github.com/matiasm15), [@maugomez77](https://github.com/maugomez77), [@maxime-fleury](https://github.com/maxime-fleury), [@mdpmcc](https://github.com/mdpmcc), [@Mfweb](https://github.com/Mfweb), [@misuadn-laplace](https://github.com/misuadn-laplace), [@MLEARNER701](https://github.com/MLEARNER701), [@MLTQ](https://github.com/MLTQ), [@mu-mei](https://github.com/mu-mei), [@Mzzj114](https://github.com/Mzzj114), [@nicu-chiciuc](https://github.com/nicu-chiciuc), [@Paulee314](https://github.com/Paulee314), [@pCwOrM](https://github.com/pCwOrM), [@rahulsundar477-star](https://github.com/rahulsundar477-star), [@rayy3535](https://github.com/rayy3535), [@RhizoNymph](https://github.com/RhizoNymph), [@rishabh-16](https://github.com/rishabh-16), [@RobertBarnettProjects](https://github.com/RobertBarnettProjects), [@sat3n](https://github.com/sat3n), [@Scratch-net](https://github.com/Scratch-net), [@SeriousRising](https://github.com/SeriousRising), [@Sethumathavanpk](https://github.com/Sethumathavanpk), [@shardmods](https://github.com/shardmods), [@Sigomi](https://github.com/Sigomi), [@sp20262026](https://github.com/sp20262026), [@surfyhou](https://github.com/surfyhou), [@t-choudhury](https://github.com/t-choudhury), [@ThatOneShortGuy](https://github.com/ThatOneShortGuy), [@TimShakespeare](https://github.com/TimShakespeare), [@TomMoeras](https://github.com/TomMoeras), [@TOTOGT](https://github.com/TOTOGT), [@Trefoiler](https://github.com/Trefoiler), [@TVSuchty](https://github.com/TVSuchty), [@twaldin](https://github.com/twaldin), [@unhingedpanda](https://github.com/unhingedpanda), [@UnityChaos](https://github.com/UnityChaos), [@user42245](https://github.com/user42245), [@varo6](https://github.com/varo6), [@vivekshivarajkumar](https://github.com/vivekshivarajkumar), [@walkingsophie](https://github.com/walkingsophie), [@whitegrave1917-web](https://github.com/whitegrave1917-web), [@WilmervH](https://github.com/WilmervH), [@WorldianAI](https://github.com/WorldianAI), [@Wronskode](https://github.com/Wronskode), [@yingluom](https://github.com/yingluom), [@zediir](https://github.com/zediir)

<!-- volunteer-roster-end -->

[Code contributors](https://github.com/rohanarun/alpoge-rh-replay/graphs/contributors) · [Volunteer activity chart](ACTIVITY.md)

### Active claims awaiting evidence

[Browse open granted claims on GitHub](https://github.com/rohanarun/alpoge-rh-replay/issues?q=is%3Aissue+is%3Aopen+label%3Aclaim-granted).

<details>
<summary>Show active claims awaiting evidence</summary>

<!-- active-volunteers-start -->

[35 entries. View the full table](tracker/volunteer-tables/active/README.md).

| Contributor | Task | Status |
|---|---|---|
| [@galakurpi](https://github.com/galakurpi) | [M137346](https://github.com/rohanarun/alpoge-rh-replay/issues/21117) | Claimed |
| [@galakurpi](https://github.com/galakurpi) | [M108927](https://github.com/rohanarun/alpoge-rh-replay/issues/21118) | Claimed |
| [@galakurpi](https://github.com/galakurpi) | [M173750](https://github.com/rohanarun/alpoge-rh-replay/issues/21119) | Claimed |
| [@mabdelazim](https://github.com/mabdelazim) | [M062140](https://github.com/rohanarun/alpoge-rh-replay/issues/22254) | Claimed |
| [@mabdelazim](https://github.com/mabdelazim) | [M062151](https://github.com/rohanarun/alpoge-rh-replay/issues/22327) | Claimed |
| [@mabdelazim](https://github.com/mabdelazim) | [M062155](https://github.com/rohanarun/alpoge-rh-replay/issues/22332) | Claimed |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M063130](https://github.com/rohanarun/alpoge-rh-replay/issues/25879) | Claimed |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M131258](https://github.com/rohanarun/alpoge-rh-replay/issues/25970) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M051277](https://github.com/rohanarun/alpoge-rh-replay/issues/26977) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M079827](https://github.com/rohanarun/alpoge-rh-replay/issues/26978) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M080139](https://github.com/rohanarun/alpoge-rh-replay/issues/26979) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M134025](https://github.com/rohanarun/alpoge-rh-replay/issues/26980) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M141042](https://github.com/rohanarun/alpoge-rh-replay/issues/26981) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M147088](https://github.com/rohanarun/alpoge-rh-replay/issues/26992) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M004289](https://github.com/rohanarun/alpoge-rh-replay/issues/26993) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M034703](https://github.com/rohanarun/alpoge-rh-replay/issues/26994) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M036491](https://github.com/rohanarun/alpoge-rh-replay/issues/27042) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M079838](https://github.com/rohanarun/alpoge-rh-replay/issues/27043) | Claimed |
| [@loremcdmx](https://github.com/loremcdmx) | [M140261](https://github.com/rohanarun/alpoge-rh-replay/issues/27044) | Claimed |
| [@emsi](https://github.com/emsi) | [M034433](https://github.com/rohanarun/alpoge-rh-replay/issues/30092) | Claimed |

<!-- active-volunteers-end -->

</details>

<details>
<summary>Submitted for review</summary>

<!-- pending-volunteers-start -->

[8,009 entries. View the full table](tracker/volunteer-tables/pending/README.md).

| Contributor | Task | Review |
|---|---|---|
| [@JamCh01](https://github.com/JamCh01) | [M089843](https://github.com/rohanarun/alpoge-rh-replay/issues/34941#issuecomment-7083643648) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M091131](https://github.com/rohanarun/alpoge-rh-replay/issues/34942#issuecomment-7083629067) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M091197](https://github.com/rohanarun/alpoge-rh-replay/issues/34943#issuecomment-7083624287) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M091487](https://github.com/rohanarun/alpoge-rh-replay/issues/34944#issuecomment-7083637060) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M093359](https://github.com/rohanarun/alpoge-rh-replay/issues/34945#issuecomment-7083630700) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M094422](https://github.com/rohanarun/alpoge-rh-replay/issues/34946#issuecomment-7083619457) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M094426](https://github.com/rohanarun/alpoge-rh-replay/issues/34947#issuecomment-7083645279) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M094973](https://github.com/rohanarun/alpoge-rh-replay/issues/34948#issuecomment-7083638690) | Pending review |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M171570](https://github.com/rohanarun/alpoge-rh-replay/issues/34949#issuecomment-7083602601) | Pending review |
| [@hipotures](https://github.com/hipotures) | [M062142](https://github.com/rohanarun/alpoge-rh-replay/issues/34950#issuecomment-7083612828) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M095459](https://github.com/rohanarun/alpoge-rh-replay/issues/34951#issuecomment-7083648550) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M095607](https://github.com/rohanarun/alpoge-rh-replay/issues/34953#issuecomment-7083646935) | Pending review |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M104709](https://github.com/rohanarun/alpoge-rh-replay/issues/34954#issuecomment-7083593361) | Pending review |
| [@hipotures](https://github.com/hipotures) | [M062889](https://github.com/rohanarun/alpoge-rh-replay/issues/34955#issuecomment-7083626505) | Pending review |
| [@JamCh01](https://github.com/JamCh01) | [M098156](https://github.com/rohanarun/alpoge-rh-replay/issues/34958#issuecomment-7083650058) | Pending review |
| [@hipotures](https://github.com/hipotures) | [M063511](https://github.com/rohanarun/alpoge-rh-replay/issues/34959#issuecomment-7083640656) | Pending review |
| [@hipotures](https://github.com/hipotures) | [M063512](https://github.com/rohanarun/alpoge-rh-replay/issues/34964#issuecomment-7083654404) | Pending review |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M107341](https://github.com/rohanarun/alpoge-rh-replay/issues/34969#issuecomment-7083641486) | Pending review |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M166291](https://github.com/rohanarun/alpoge-rh-replay/issues/34970#issuecomment-7083632310) | Pending review |
| [@hipotures](https://github.com/hipotures) | [M066593](https://github.com/rohanarun/alpoge-rh-replay/issues/34972#issuecomment-7083668704) | Pending review |

<!-- pending-volunteers-end -->

</details>

<details>
<summary>Reviewed builds</summary>

<!-- volunteers-start -->

[15,270 entries. View the full table](tracker/volunteer-tables/reviewed/README.md).

| Contributor | Task | Modules | Review |
|---|---|---:|---|
| [@gilad12-coder](https://github.com/gilad12-coder) | [M123501](https://github.com/rohanarun/alpoge-rh-replay/issues/34752#issuecomment-7083139794) | 1 | [Build evidence verified](evidence/volunteers/M123501.json) |
| [@JamCh01](https://github.com/JamCh01) | [M034792](https://github.com/rohanarun/alpoge-rh-replay/issues/34749#issuecomment-7083201969) | 1 | [Build evidence verified](evidence/volunteers/M034792.json) |
| [@JamCh01](https://github.com/JamCh01) | [M032791](https://github.com/rohanarun/alpoge-rh-replay/issues/34748#issuecomment-7083208342) | 1 | [Build evidence verified](evidence/volunteers/M032791.json) |
| [@BenCaunt](https://github.com/BenCaunt) | [M142750](https://github.com/rohanarun/alpoge-rh-replay/issues/34747#issuecomment-7083127369) | 1 | [Build evidence verified](evidence/volunteers/M142750.json) |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M066573](https://github.com/rohanarun/alpoge-rh-replay/issues/34612#issuecomment-7082847708) | 1 | [Build evidence verified](evidence/volunteers/M066573.json) |
| [@gilad12-coder](https://github.com/gilad12-coder) | [M133709](https://github.com/rohanarun/alpoge-rh-replay/issues/34611#issuecomment-7082856943) | 1 | [Build evidence verified](evidence/volunteers/M133709.json) |
| [@hipotures](https://github.com/hipotures) | [M164961](https://github.com/rohanarun/alpoge-rh-replay/issues/34605#issuecomment-7082869098) | 1 | [Build evidence verified](evidence/volunteers/M164961.json) |
| [@JamCh01](https://github.com/JamCh01) | [M113390](https://github.com/rohanarun/alpoge-rh-replay/issues/34600#issuecomment-7082859181) | 1 | [Build evidence verified](evidence/volunteers/M113390.json) |
| [@JamCh01](https://github.com/JamCh01) | [M104114](https://github.com/rohanarun/alpoge-rh-replay/issues/34599#issuecomment-7082865585) | 1 | [Build evidence verified](evidence/volunteers/M104114.json) |
| [@JamCh01](https://github.com/JamCh01) | [M099981](https://github.com/rohanarun/alpoge-rh-replay/issues/34592#issuecomment-7082870312) | 1 | [Build evidence verified](evidence/volunteers/M099981.json) |
| [@JamCh01](https://github.com/JamCh01) | [M099961](https://github.com/rohanarun/alpoge-rh-replay/issues/34591#issuecomment-7082869113) | 1 | [Build evidence verified](evidence/volunteers/M099961.json) |
| [@hipotures](https://github.com/hipotures) | [M164960](https://github.com/rohanarun/alpoge-rh-replay/issues/34586#issuecomment-7082841493) | 1 | [Build evidence verified](evidence/volunteers/M164960.json) |
| [@JamCh01](https://github.com/JamCh01) | [M099070](https://github.com/rohanarun/alpoge-rh-replay/issues/34585#issuecomment-7082834381) | 1 | [Build evidence verified](evidence/volunteers/M099070.json) |
| [@hipotures](https://github.com/hipotures) | [P2105](https://github.com/rohanarun/alpoge-rh-replay/issues/32213#issuecomment-7079033098) | 64 | [Build evidence verified](evidence/volunteers/P2105.json) |
| [@hipotures](https://github.com/hipotures) | [P2077](https://github.com/rohanarun/alpoge-rh-replay/issues/32148#issuecomment-7078841023) | 64 | [Build evidence verified](evidence/volunteers/P2077.json) |
| [@JamCh01](https://github.com/JamCh01) | [P2814](https://github.com/rohanarun/alpoge-rh-replay/issues/32081#issuecomment-7078705646) | 11 | [Build evidence verified](evidence/volunteers/P2814.json) |
| [@RhizoNymph](https://github.com/RhizoNymph) | [P2748](https://github.com/rohanarun/alpoge-rh-replay/issues/25103#issuecomment-7085656907) | 64 | [Build evidence verified](evidence/volunteers/P2748.json) |
| [@UnityChaos](https://github.com/UnityChaos) | [P2771](https://github.com/rohanarun/alpoge-rh-replay/issues/30424#issuecomment-7088754643) | 64 | [Build evidence verified](evidence/volunteers/P2771.json) |
| [@hipotures](https://github.com/hipotures) | [M164958](https://github.com/rohanarun/alpoge-rh-replay/issues/34579#issuecomment-7082827663) | 1 | [Build evidence verified](evidence/volunteers/M164958.json) |
| [@JamCh01](https://github.com/JamCh01) | [M094425](https://github.com/rohanarun/alpoge-rh-replay/issues/34578#issuecomment-7082829494) | 1 | [Build evidence verified](evidence/volunteers/M094425.json) |

<!-- volunteers-end -->

</details>

## Completed parts

<!-- completed-start -->

| Evidence for distinct module IDs | Count |
|---|---:|
| Successful source build observed | 26,591 |
| Pilot proof object reused | 150 |
| Pilot downstream module kernel-checked | 1 |
| Distributed proof object reused | 16,970 |
| Volunteer build evidence reviewed | 65,935 |
| Worker target kernel replay reviewed | 72 |
| **Total with recorded module evidence** | **109,719 / 175,187** |

[See each completed part and its evidence](completed/README.md) · [Machine-readable ledger](tracker/completed.tsv)

<!-- completed-end -->

## Give this prompt to an agent

**Default: verify, port or optimize grh-lean.**

> Help verify and optimize the short Lean proof of RH/GRH at https://github.com/lsernau/grh-lean (copied, at Lean v4.37.0-rc1, into the `grh/` folder of https://github.com/rohanarun/alpoge-rh-replay; send PRs there). Read https://github.com/rohanarun/alpoge-rh-replay/blob/main/auto-research.md and pick one task: an independent build plus `lake comparator`, a Lean v4.37.0-rc1 port fix, or an optimization (profile slow files, flatten-simplify-refold proofs, remove dead lemmas, narrow imports). Check open PRs on rohanarun/alpoge-rh-replay first, then open a draft PR to claim your file.
>
> **Strict rules:** never modify `Challenge.lean`, `src/Statements.lean` or `comparator.json`; never add `sorry`, `admit`, axioms, `native_decide` or unsafe features; don't raise `maxHeartbeats` to hide a problem; build with `LEAN_ABORT_ON_PANIC=1` and keep `#print axioms` to `propext`, `Classical.choice`, `Quot.sound`. Include before/after build times for optimizations.

[Agent instructions](AGENTS.md) · [grh/ folder](grh/) · [PR #120 (paused)](https://github.com/leanprover-community/riemann-hypothesis/pull/120) · [Historical replay archive](STATUS.md)

## Reproduce the check

On Linux, install the elan launcher and ensure its `lean` and `lake` commands are on your PATH. The script also requires Python 3.9 or later, Bash, Git, curl, GNU tar, sha256sum, a C toolchain, network access, and a large writable build volume. Run from this repository with a fresh output directory.

```bash
./verify.sh /path/to/empty/replay-directory
```

The script compares every archive part with its SHA-256 digest, checks the toolchain and mathlib revision, builds the final module from source, and writes the transcript to `replay.log` in the output directory. The pinned Lean compiler is 4.33.1 and the mathlib commit is `0df444a360eaa60ab8c11dca51a86af692955474`.

### Integrity checkpoints

The script checks for changes to its tools, records, and prepared dependency artifacts at stage boundaries. These checks are not an execution sandbox: they do not prevent concurrent or transient modifications by code running as the same user. In execution order:

1. **Archive verification.** Every downloaded archive part is checked against `parts.sha256` with `sha256sum -c`. The SHA-256 digests of `Audit.lean`, `parts.sha256`, and `audit/dependency-artifacts.py` are recorded before any archive code runs.
2. **Manifest pin.** Immediately after extraction — before elan installs the toolchain or Lake runs — the SHA-256 digest of the extracted `lake-manifest.json` is recorded.
3. **Toolchain integrity.** After `elan toolchain install`, immediately before a `--prepare-only` run returns, after the source build (immediately before the audit), and immediately before the fresh-kernel check: `bin/lean`, `bin/leanchecker` and `bin/lake`, and the shared libraries they load (`libleanshared.so`, `libLake_shared.so`, `libleanshared_1.so`, `libleanshared_2.so`, `libInit_shared.so`), still match the digests pinned in `verify.sh` from the official Lean 4.33.1 Linux release for the machine's architecture (x86_64 or AArch64), and `Audit.lean` and `parts.sha256` still match the digests recorded at step 1. Prints `REPLAY_INTEGRITY_CHECK_PASSED`.
4. **Dependency check.** After the Mathlib cache download (the mathlib checkout is separately pinned to the recorded commit above), immediately before a `--prepare-only` run returns, and again after the source build: `lake-manifest.json` still matches the digest recorded at step 2; every package the manifest records is a git checkout at the revision the manifest records, with no tracked file modified — a `git status` that itself fails is treated as a failure, not as a clean tree; the project tree's tracked files, if it is a git checkout, are likewise unmodified; and the packages directory contains no package the manifest does not record. Prints `REPLAY_DEPENDENCIES_PRISTINE_PASSED`.
5. **Prepared artifact baseline.** Before the project source build, `dependency-artifacts.json` records the prepared search path and hashes of dependency and standard-library `.olean`, `.olean.server`, `.olean.private`, `.ir`, `.ir.sig`, and `.so` files. The parent verifier retains the snapshot digest. Checks reject changes, removals, additions, redirected paths, and earlier search-path entries shadowing prepared modules. Generated setup inputs and traces are excluded. Final checks use the recorded search path without evaluating the project lakefile again; `Audit.lean` explicitly imports Mathlib before Main. Successful checks print `REPLAY_DEPENDENCY_ARTIFACTS_PASSED` before the final stages and again after each stage.

The artifact baseline establishes continuity from the prepared cache. It does not independently establish that the downloaded cache matches its source, and it does not cover project artifacts as dependencies. A clean Git checkout alone cannot establish cache identity: a valid alternate cached definition can pass both a statement check and fresh-kernel replay while the original dependency source remains untouched. The native regression in `tests/dependency-artifacts-native.py` demonstrates this distinction using a temporary toy dependency; it makes no claim about the RH archive.

## Read the evidence

1. `REPLAY_SOURCE_BUILD_PASSED` means Lake built the module containing the final theorem.
2. `REPLAY_AXIOM_AUDIT_PASSED` means the five public theorems in `Main` type-checked against their statements, which `Audit.lean` writes out with Mathlib definitions only. The audit rejects any reported axiom beyond propositional extensionality, classical choice, and quotient soundness.
3. `REPLAY_FRESH_KERNEL_PASSED` means Lean’s checker replayed the declarations imported by `Main` in a fresh environment. It uses the same Lean kernel implementation.

The integrity markers have separate scopes. `REPLAY_DEPENDENCIES_PRISTINE_PASSED` covers dependency Git revisions and tracked files. `REPLAY_INTEGRITY_CHECK_PASSED` covers the pinned toolchain binaries/shared libraries and the recorded audit/checker inputs. `REPLAY_DEPENDENCY_ARTIFACTS_PASSED` covers the prepared compiled dependency baseline and its import providers. None of these markers alone establishes the full proof result.

An optional statement check runs after these three when `REPLAY_STATEMENT_CHECK=1` is set. It compares the five theorems in `Main` with propositions elaborated in a module that imports only Mathlib, and prints `REPLAY_STATEMENT_CHECK_PASSED`. It can also be run against a completed checkout; see [audit/README.md](audit/README.md).

A completed report should include the exit status, all three outputs, the printed theorem and axioms, and a checksum for the archived transcript. A machine or storage failure leaves the mathematical claim unresolved.

## Optional determinant check

The [M115707 example](examples/M115707/README.md) compares a shorter local Gram determinant argument with the published module. This check runs separately from the volunteer replay.

## Volunteer activity

![Cumulative chart of volunteers, granted claims, and replay submissions](tracker/activity.svg)

[How the chart is counted](ACTIVITY.md) · [Event data](tracker/activity.tsv)

## License

The original replay tooling and documentation in this repository are available under the [MIT License](LICENSE). Upstream Lean source, Mathlib, and third-party artifacts retain their respective licenses.
