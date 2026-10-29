# Development documentation changelog / Änderungen

## 2026-10-29 – Candidate documentation refresh (not a release)

- Added full German and English walkthroughs for installation, APS, LEGS, ASS, AD destination migration and troubleshooting.
- Documented two mod ZIPs containing three systems; current manual service options, repair lift behavior, refuel/charge limits, local receipt printing and audio rules.
- Distinguished **installed** APS + SmartGate from **canonical APS without resume**, **29 October SmartGate candidate not installed**, and historical staging.
- Documented SmartGate target-ID change: name+X/Z identity, conservative UNKNOWN/fail-closed behavior, one-time legacy AD destination re-selection, and still-pending native tests.
- Clarified current LEGS gate trigger colors/pre-opening formula, bay physical state vs reservation, return routing and service queue limitations.
- No runtime sources or archives changed; no version increment, public release or tag.

See [candidate build matrix](docs/BUILD_STATUS.md). This changelog describes documentation/candidates, **not a published stable 1.0**.


## 2026-10-29 – Illustrated documentation proposal

- Added matching DE/EN source-derived illustrations to existing APS, LEGS, ASS, installation, migration and troubleshooting guides.
- Added a screened image inventory, provenance, lossless optimization sizes and explicit missing-native-screenshot list.
- Updated local SmartGate installation status to the later `SG_InteractionDescription_20261029` candidate; native target-identity verification remains pending.
- Documentation only: no mod ZIPs, runtime changes, release, tag or deployment.
