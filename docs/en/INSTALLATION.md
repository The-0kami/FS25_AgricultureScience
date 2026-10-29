# Installation and updates – Agriculture Science

> **As of 29 October 2026:** Documentation for development candidates, **not a release** in this repository. The latest SmartGate AD target identity fix is **not installed or verified in-game**. See [build status](../BUILD_STATUS.md).

## Packages and prerequisites

There are **two** mod ZIPs: `FS25_APS_AgricultureScience.zip` (APS **plus ASS**) and `FS25_SmartGate_AgricultureScience.zip` (LEGS). AutoDrive is required for automated driving (reference **3.0.1.4**, not included). Basic APS parking and SmartGate gate controls can work independently; **ASS service execution requires both mods**. Courseplay is optional.

## Single-player setup

1. Completely exit FS25. **Back up your savegame and existing mod files.**
2. Unpack an outer bundle **only if one was actually supplied**. Otherwise use the two individual mod ZIPs. GitHub source-code archives are not installable FS25 mods.
3. Copy both **unmodified ZIPs** to the active mods folder. Do not extract the individual mod ZIPs. Remove parallel older ZIPs or unpacked folders using the same mod names.
4. Install AutoDrive separately, enable the relevant mods in the savegame, and verify your AutoDrive network.
5. Open the shared **Agriculture Science** tab and check APS, LEGS, ASS and Audio views. Unavailable module pages may be disabled.
6. For services, configure a supported native service source and bay in LEGS first; test one manual ASS service before enabling automation. See [ASS tutorial](TUTORIAL_ASS.md).

## Dedicated server

1. Stop the server. Back up the savegame, installed mod ZIPs and the **server's `smartGate.xml`**.
2. Use **identical mod ZIP files** and compatible AutoDrive builds on the server and all clients.
3. Compare **SHA-256 hashes**, not only `1.0.0.0` version labels: several candidate builds share that version. See [build status](../BUILD_STATUS.md).
4. Check farm permissions, native service sources, bay reservations and AD routing. The full current package is **not yet Dedi-verified**.

## Updating an existing installation

1. Record current ZIP hashes and create backups.
2. Select a compatible pair of ZIPs; do not leave duplicate versions installed.
3. Verify existing gates, triggers, service sources and AD destinations in your savegame.
4. **Only for the not-yet-installed SmartGate candidate dated 29 October:** Re-select every legacy bay AD destination with a positive index from the live list once, to capture its name and coordinates. Do not silently trust a stale index. See [migration guide](MIGRATION_AD_TARGETS.md).
5. Test a single vehicle and bay before enabling automated jobs.

## External sound packs

Custom voice packs live outside the mod ZIP at `modSettings/APS_sounds/voices/`. Back up custom edits before updating. Existing external default voice files are not blindly overwritten. Private packs are not part of a public release.

## Notes

FS25 `1.25.0.0` is a documented test version, **not a proven universal minimum**. Do not describe the new target identity fix as functional in-game before installation and native tests.
