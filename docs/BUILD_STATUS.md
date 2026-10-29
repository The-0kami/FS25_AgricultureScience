# Build- und Teststatus / Build and test status

> **Stand / As of 29 October 2026.** Die Hashes wurden **von Codex anhand lokaler ZIP-Dateien berichtet**; dieses öffentliche Dokument ist **keine Remote-Binärprüfung**. Alle untenstehenden Mod-Descriptoren melden `1.0.0.0`. **Gleiche Versionsnummer ≠ gleicher Build.**

| Rolle / Role | ZIP | SHA-256 | Bytes | Native verification |
|---|---|---|---:|---|
| **Installiert / Installed** APS mit Resume-Experiment | `FS25_APS_AgricultureScience.zip` | `c53cf018628659c3bac29a1eec83dfb731070dfa49f553730be1c3dc60e0b202` | 33985052 | Nutzer meldet erfolgreiche SP-Läufe / successful user-reported SP runs; no full Dedi approval |
| **Installiert / Installed** SG (GUI-Fix 28.10.) | `FS25_SmartGate_AgricultureScience.zip` | `230fd8cb453585dd854460d707828d3a9759af4a4a805abad9585e867e176d65` | 2398508 | Rename dialog user-confirmed SP + Dedi; not full pack verification |
| **Neuester Kandidat / Latest candidate** SG AD-Zielidentität (29.10.) | `FS25_SmartGate_AgricultureScience.zip` | `622b7772d016ed4116133f146ce6aea6023a8cc0ae8b754b4794dd96db291570` | 2400527 | **NOT INSTALLED; automated tests only; no SP/Dedi verification** |
| Kanonischer APS-Export **ohne** Resume | `FS25_APS_AgricultureScience.zip` | `37a9dd175b4de8d4693ad0d93114fdf654da59545f0fc0124cdb97b4d3e92c99` | 33982316 | Not equivalent to installed experimental APS |
| Ältere heruntergeladene SG-Datei / Older downloaded SG file | `FS25_SmartGate_AgricultureScience (1).zip` | `238bfd2f603215ff49acada1325d675dc72e7d88d8e3ff9ed6953117ffdd51c5` | 2398306 | GUI rename input/footer fixes missing; remote branch was **not** inspected in Codex handoff |

## Historisches Staging / Historical staging

Das Release-Staging-Manifest vom **26.10.2026** bezeichnet `CANONICAL_WITHOUT_RESUME_EXPERIMENT`, darunter APS `54ac2bc90ebf4f8cc3a5048abcb78cdde2062d05833b6d60644bdfcb9142a9d4` und äußeres Paket `b07066b06bbf445caf746a29f3a48f6c8aa230aaa6442c329a469220ca639ce8`. **Nicht als heutige ZIP-Hashes verwenden.** / Do not reuse these as current build hashes.

## Verifikation / Verification

- SHA-256, descriptors and ZIP CRC were inspected locally by Codex (reported, not independently re-run here).
- Registered APS + SG regression suites and new AD-target identity cases passed, including target-index shift, ambiguity, legacy data, save/reload, stale client and lease cancellation.
- Existing **70 work-service/lift** and **31 AD task-boundary** cases passed in automated tests.
- **Simulation is not native GIANTS/C++/rendering/Dedi proof.** The 29 October target identity candidate remains **untested in-game**.
- No binary publication, tag or new package release is authorized by this documentation update.

## Hinweise / Notes

AutoDrive **3.0.1.4** is the tested reference. Game version **1.25.0.0** is a documented test environment, not a proven minimum. `N.E.C.K.` camera project and Mass Maintenance Protocol are planned separately, **not included**.

Weitere Dokumentation / Further reading: [Deutsch](de/INSTALLATION.md) · [English](en/INSTALLATION.md) · [AD-Zielmigration DE](de/MIGRATION_AD_TARGETS.md) · [AD target migration EN](en/MIGRATION_AD_TARGETS.md).
