# Agriculture Science Pack

**Farming Simulator 25 · Documentation for development candidates / Dokumentation der Testkandidaten**

[Deutsch](#deutsch) | [English](#english) | [Builds & SHA-256](docs/BUILD_STATUS.md)

## Deutsch

**Zwei ZIPs, drei Systeme:** `FS25_APS_AgricultureScience.zip` enthält **A.P.S. – Advanced Parking Sequence** und **A.S.S. – Autonomous Service Supervisor**. `FS25_SmartGate_AgricultureScience.zip` enthält **L.E.G.S. – Logical Entrance Guidance System**.

- **APS:** Bis zu zwei direkt angehängte Geräte zu AutoDrive-Parkzielen bringen, abkuppeln, danach Fahrzeug parken; unterstützte manuelle und Jobende-Übergänge.
- **LEGS:** Tore/Interactables, individuelle Trigger und Sicherheitszonen, AD-Voröffnung, Provider und Service-Bays.
- **ASS:** Unterstützte WASH-, REPAIR-/Hebebühnen- und REFUEL-/CHARGE-Services, Bay-Reservierungen und Serviceübergaben, optionale private Ticketdrucker-Anzeige.

**Status: Entwicklungs-/Preview-Dokumentation – keine finale 1.0-Freigabe.** Der SmartGate-Kandidat `SG_InteractionDescription_20261029` enthält die stabile AD-Zielidentität und die bereinigte Interactive-Beschreibungszeile. Er ist **lokal installiert und automatisiert geprüft, aber noch nicht im Spiel/Dedi bestätigt**. Das ist keine Aussage über die Installation auf fremden Servern. Bestehende Bay-Ziele müssen einmal neu ausgewählt werden. Gleiche Modversion `1.0.0.0` bedeutet nicht bytegleiche ZIPs. [Details und Prüfsummen](docs/BUILD_STATUS.md).

**Voraussetzungen:** LS25 (Teststand 1.25.0.0), AutoDrive (Referenz 3.0.1.4) für Fahrten, beide AS-Mods für ASS-Service; Courseplay optional. Nicht alle Gebäude, Energietypen, Geräte oder MP-Fälle sind abgenommen.

### Anleitungen auf Deutsch

- [Installation, Update, Dedicated Server](docs/de/INSTALLATION.md)
- [APS: Parken und Abkuppeln](docs/de/TUTORIAL_APS.md)
- [LEGS: Tore, Trigger und Safety](docs/de/TUTORIAL_LEGS.md)
- [ASS: Service-Bays, WASH, REPAIR und REFUEL](docs/de/TUTORIAL_ASS.md)
- [AD-Zielmigration für neueren SG-Kandidaten](docs/de/MIGRATION_AD_TARGETS.md)
- [Fehlerdiagnose und Bugreports](docs/de/TROUBLESHOOTING.md)
- [Bildnachweis und UI-Galerie](docs/UI_CATALOG.md)
- [Buildstatus und Hashes](docs/BUILD_STATUS.md)

## English

**Two ZIPs, three systems:** `FS25_APS_AgricultureScience.zip` includes **A.P.S. – Advanced Parking Sequence** plus **A.S.S. – Autonomous Service Supervisor**. `FS25_SmartGate_AgricultureScience.zip` includes **L.E.G.S. – Logical Entrance Guidance System**.

- **APS:** Drive up to two suitable directly attached implements to AutoDrive parking destinations, detach, then park the vehicle; supported manual and job-end interception.
- **LEGS:** Gates/interactables, configurable trigger and safety regions, AD pre-opening, service providers and bays.
- **ASS:** Supported WASH, REPAIR/lift and REFUEL/CHARGE services, bay reservations, service handoff and optional private printer receipts.

**Status: development/preview documentation, not a final 1.0 release.** SmartGate candidate `SG_InteractionDescription_20261029` contains stable AD destination identity and the cleaned-up interactable description row. It is **locally installed and automatically tested, but not yet verified in-game/on Dedi**. This does not describe deployment to other servers. Existing bay destinations require one deliberate re-selection. The shared mod version `1.0.0.0` does not mean identical binaries. See [build matrix](docs/BUILD_STATUS.md).

**Requirements:** FS25 (documented test 1.25.0.0), AutoDrive (reference 3.0.1.4) for driving, both AS mods for ASS services; Courseplay optional. Not every building, energy type, implement or multiplayer case is verified.

### English guides

- [Install, update and dedicated servers](docs/en/INSTALLATION.md)
- [APS: parking and detaching](docs/en/TUTORIAL_APS.md)
- [LEGS: gates, triggers and safety](docs/en/TUTORIAL_LEGS.md)
- [ASS: bays, WASH, REPAIR and REFUEL](docs/en/TUTORIAL_ASS.md)
- [AD destination migration for newer SG candidate](docs/en/MIGRATION_AD_TARGETS.md)
- [Troubleshooting and bug reports](docs/en/TROUBLESHOOTING.md)
- [Image provenance and UI gallery](docs/UI_CATALOG.md)
- [Build status and hashes](docs/BUILD_STATUS.md)

## Downloads / Veröffentlichungen

**In diesem Repository wurden noch keine Mod-ZIPs oder Releases veröffentlicht. / No mod ZIPs or releases have been published in this repository yet.** A GitHub auto-generated source archive is not an installable game mod. [Releases](../../releases) will be used only after separate approval.

## Rechte / Rights

Default voice/music redistribution was confirmed by the project owner; this does **not** authorize sharing private voice packs or unrelated media. CC0 printer SFX have separately documented source credits. Third-party code/graphic notices must be respected. **No blanket license is granted for all project assets.**

## Feedback

Use [GitHub Issues](../../issues) with the **actual ZIP SHA-256**, game/AD versions, SP/MP/Dedi context, reproducing steps and a **redacted** current log.

*Agriculture Science – Automate smarter. Farm better.*

