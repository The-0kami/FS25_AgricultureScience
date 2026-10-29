# Agriculture Science Pack

**Farming Simulator 25 · Documentation for development candidates / Dokumentation der Testkandidaten**

[Deutsch](#deutsch) | [English](#english) | [Builds & SHA-256](docs/BUILD_STATUS.md)

## Deutsch

**Drei Systeme, ein gemeinsamer Ablauf.** Agriculture Science verbindet automatisiertes Fahrzeugparken, intelligente Torsteuerung und autonome Fahrzeugwartung.

- **A.P.S. – Advanced Parking Sequence:** Koordiniert AutoDrive-Parkabläufe, das Abstellen und Abkuppeln von bis zu zwei direkt angehängten Geräten sowie die anschließende Fahrzeugparkfahrt.
- **L.E.G.S. – Logical Entrance Guidance System:** Steuert Tore und Interactables und stellt die Infrastruktur mit Servicebereichen, Bays und Reservierungen bereit.
- **A.S.S. – Autonomous Service Supervisor:** Verbindet Fahrzeugabläufe und Serviceinfrastruktur, um unterstützte Wasch-, Reparatur-, Tank- und Ladevorgänge zu koordinieren. Optional zeigt es lokale Servicebelege an.

**Technischer Paketinhalt:** Zwei Mod-ZIPs: `FS25_APS_AgricultureScience.zip` (mit A.S.S.-Steuerlogik) und `FS25_SmartGate_AgricultureScience.zip` (L.E.G.S.-Serviceinfrastruktur). Für A.S.S.-Services arbeiten beide zusammen.

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

**Three systems. One workflow.** Agriculture Science brings together automated vehicle parking, intelligent gate control and autonomous servicing.

- **A.P.S. – Advanced Parking Sequence:** Coordinates AutoDrive parking, detaching up to two suitable directly attached implements, and driving the vehicle to its parking destination.
- **L.E.G.S. – Logical Entrance Guidance System:** Controls gates and interactables and provides service-area infrastructure, bays and reservations.
- **A.S.S. – Autonomous Service Supervisor:** Connects vehicle workflows with service infrastructure to coordinate supported washing, repair, refueling and charging. Optional local service receipts are available.

**Technical package contents:** Two mod ZIPs: `FS25_APS_AgricultureScience.zip` (including ASS coordination logic) and `FS25_SmartGate_AgricultureScience.zip` (LEGS service infrastructure). Both are used together for ASS services.

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

