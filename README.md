# Agriculture Science – Farming Simulator 25

**Modulare Automatisierung und Kamera-Werkzeuge für Farming Simulator 25.**  
**Modular automation and camera tools for Farming Simulator 25.**

[Deutsch](#deutsch) · [English](#english) · [Release preparation / Release-Vorbereitung](docs/RELEASE_PREPARATION.md) · [Historische Build-Matrix](docs/BUILD_STATUS.md)

> **Release-Vorbereitung / Release preparation – 14.11.2026:** Lokaler Stand vom Nutzer bestätigt; **keine Release-Freigabe**. Local versions and candidate SHA-256 hashes are documented below; they are **not approved downloads**. October 2026 build notes remain historical.

## Deutsch

Agriculture Science besteht aus **unabhängig installierbaren Modulen**. Jedes Modul bringt laut aktuellem Projektstand seine eigene Menü-/UI-Integration mit. Es ist keine zusätzliche gemeinsame GUI-Mod vorgesehen.

| Modul | Zweck | Verteilung |
|---|---|---|
| **A.P.S. – Advanced Parking Sequence** | Koordiniert AutoDrive-Parkabläufe und unterstützte Geräte-/Fahrzeugübergaben | Eigenständige Mod-ZIP |
| **A.S.S. – Autonomous Service Supervisor** | Koordiniert unterstützte Wasch-, Reparatur-, Tank-/Ladeabläufe und Serviceanzeigen | **Bestandteil von A.P.S.**, keine eigene ZIP |
| **L.E.G.S. – Logical Entrance Guidance System** | Tore, Interaktionen und Infrastruktur für Servicebereiche, Bays und Reservierungen | Eigenständige Mod-ZIP mit technischer SmartGate-Identität |
| **N.E.C.K. – New External Camera Kit** | Eigenständige Kameramod mit Kameraperspektiven und Aufnahmen im AutoDrive-Fahrkontext | Eigenständige Mod-ZIP |
| **H.E.A.D. – Heuristic Environmental Analysis Drone** | Separate Drohnen-/Scan-Mod, derzeit in Entwicklung | **Nicht Teil des ersten Releases** |

**Geplante Downloads (noch nicht veröffentlicht):** Einzel-ZIPs für A.P.S. (inkl. A.S.S.), L.E.G.S. und N.E.C.K.; zusätzlich ein **Komplettpaket**, das dieselben unveränderten Mod-ZIPs enthält. Das Komplettpaket muss vor der Installation **entpackt** werden; nur die einzelnen installierbaren Mod-ZIPs gehören in den aktiven Mods-Ordner.

### Bestätigter lokaler Stand – 14.11.2026

Vom Nutzer bestätigte lokale Installation; Archive und Prüfsummen wurden im Rahmen dieser Dokumentationsänderung nicht unabhängig geprüft. **Lokale Testkandidaten, keine freigegebenen Downloads.**

| Modul / Module | Version | ZIP | SHA-256 |
|---|---|---|---|
| A.P.S. (inkl. A.S.S. und Audio / incl. A.S.S. and audio) | 1.0.0.0 | `FS25_APS_AgricultureScience.zip` | `5072b6720ead3e59e13269086267cb2cdba0e6f52b3a265e94634f1abc7c3294` |
| L.E.G.S. | 1.0.0.0 | `FS25_SmartGate_AgricultureScience.zip` | `d1c2e313021b57307d0b7d24a3cb3bf4633e55d696f80faa050a127a617db679` |
| N.E.C.K. | 0.1.0.0 | `FS25_NECK_AgricultureScience.zip` | `07d3e10fbdd603b19901d835cd422ca5632263cb1db11b4082591b08d770c41f` |

**Abhängigkeiten:** AutoDrive **3.0.1.4** ist die verwendete Referenz, keine daraus abgeleitete Mindestversion. AutoDrive ist separat zu installieren. N.E.C.K.-Filmfahrten benötigen aktives AutoDrive; die Vorschau funktioniert im besetzten Fahrzeug ohne aktives AutoDrive. L.E.G.S.-Torsteuerung läuft eigenständig; AutoDrive-Voröffnung ist optional. Die A.S.S.-Ansicht setzt geladenes A.P.S.+L.E.G.S. und eine registrierte Ansicht voraus.

**Tutorials und Host:** Alle drei Mods enthalten den gemeinsamen Host; der Host-Umbau erfolgte einmalig und koordiniert. Tourtexte und Gruppen stammen jetzt aus den Einstellungsmodulen. Fehlende Module sind ausgegraut und werden im Deep Dive übersprungen. Laut Nutzer bestanden die Lua-Tests für Teilinstallationen, fehlende/inkompatible Tourdaten und den Austausch eines Modultexts bei gleichem Host. Die modulare Tour muss noch im Spiel geprüft werden.

**L.E.G.S. neu:** „Serviceplätze → Beispiel“ erklärt einen Bereich gegenüber zwei Bays. Quelle und AD-Haltepunkt werden direkt in der Welt dargestellt; eigenes Kraftfeld und lokale Farben erscheinen auf den L.E.G.S./A.S.S.-Karten. Die neuesten Effekte sind noch im Spiel zu prüfen.

**Separat in Entwicklung:** H.E.A.D. **0.1.0.0** mit 6,9 Sekunden Startanimation, neuem räumlichem Scan, Ergebnisbox am Feld und bis zu acht überlappenden Scanflächen pro Flug; visueller Ingame-Test offen. DevTools **0.5.0.0** ist ein internes Diagnosewerkzeug. Beide gehören nicht ins öffentliche Dreierpaket.

- [Release-Konzept und offene Freigabepunkte](docs/RELEASE_PREPARATION.md)
- [Deutsch: bisherige Installation](docs/de/INSTALLATION.md) · [APS](docs/de/TUTORIAL_APS.md) · [LEGS](docs/de/TUTORIAL_LEGS.md) · [ASS](docs/de/TUTORIAL_ASS.md)
- [UI-Bildherkunft und ältere Dokumentationsgrafiken](docs/UI_CATALOG.md)
- [Historische Build-/SHA-256-Nachweise](docs/BUILD_STATUS.md)

## English

Agriculture Science is a set of **independently installable mods**. According to the current project status, each module carries its own menu/UI integration; there is no separate shared UI mod to install.

| Module | Purpose | Distribution |
|---|---|---|
| **A.P.S. – Advanced Parking Sequence** | Coordinates AutoDrive parking and supported implement/vehicle hand-offs | Standalone mod ZIP |
| **A.S.S. – Autonomous Service Supervisor** | Coordinates supported wash, repair, refuel/charge flows and service displays | **Included in A.P.S.**, not a separate ZIP |
| **L.E.G.S. – Logical Entrance Guidance System** | Gates, interactions, service infrastructure, bays and reservations | Standalone mod ZIP; internal SmartGate identity |
| **N.E.C.K. – New External Camera Kit** | Standalone camera mod for camera perspectives and recordings during AutoDrive driving | Standalone mod ZIP |
| **H.E.A.D. – Heuristic Environmental Analysis Drone** | Separate drone/scan project currently in development | **Not included in the first release** |

**Planned downloads (not published yet):** Individual ZIP files for A.P.S. (including A.S.S.), L.E.G.S. and N.E.C.K., plus a **Complete Package** containing those same unmodified ZIP files. Extract the outer Complete Package first; install only the individual mod ZIPs into the active mods directory.

### Confirmed local status – 14 November 2026

User-confirmed local installation; archives and checksums were not independently verified as part of this documentation change. **Local test candidates, not approved downloads.**

| Modul / Module | Version | ZIP | SHA-256 |
|---|---|---|---|
| A.P.S. (inkl. A.S.S. und Audio / incl. A.S.S. and audio) | 1.0.0.0 | `FS25_APS_AgricultureScience.zip` | `5072b6720ead3e59e13269086267cb2cdba0e6f52b3a265e94634f1abc7c3294` |
| L.E.G.S. | 1.0.0.0 | `FS25_SmartGate_AgricultureScience.zip` | `d1c2e313021b57307d0b7d24a3cb3bf4633e55d696f80faa050a127a617db679` |
| N.E.C.K. | 0.1.0.0 | `FS25_NECK_AgricultureScience.zip` | `07d3e10fbdd603b19901d835cd422ca5632263cb1db11b4082591b08d770c41f` |

**Dependencies:** AutoDrive **3.0.1.4** is the reference used, not an inferred minimum version. Install AutoDrive separately. N.E.C.K. filming drives require active AutoDrive; preview works in an occupied vehicle without active AutoDrive. L.E.G.S. gate control works independently; AutoDrive pre-opening is optional. The A.S.S. view requires loaded A.P.S.+L.E.G.S. and a registered view.

**Tutorials and host:** All three mods carry the shared host; its refactoring was a single coordinated change. Tour text and groups now come from the settings modules. Missing modules are greyed out and skipped by Deep Dive. The user reports passing Lua tests for partial installations, missing/incompatible tour data, and replacing a module text while retaining the same host. The modular tour still needs in-game verification.

**New in L.E.G.S.:** “Service spaces → Example” explains one area versus two bays. The source and AD stopping point are shown directly in the world; a dedicated force field and local colours appear on the L.E.G.S./A.S.S. maps. The latest effects still need in-game verification.

**Separate development:** H.E.A.D. **0.1.0.0** has a 6.9-second start animation, a new spatial scan, a result box at the field, and up to eight overlapping scan areas per flight; visual in-game testing is pending. DevTools **0.5.0.0** is an internal diagnostic tool. Neither belongs in the public three-mod package.

- [Release preparation and pending checks](docs/RELEASE_PREPARATION.md)
- [English: previous installation guide](docs/en/INSTALLATION.md) · [APS](docs/en/TUTORIAL_APS.md) · [LEGS](docs/en/TUTORIAL_LEGS.md) · [ASS](docs/en/TUTORIAL_ASS.md)
- [Image provenance / older UI documentation](docs/UI_CATALOG.md)
- [Historical build and SHA-256 records](docs/BUILD_STATUS.md)

## Downloads / Releases

**No installable release has been published here yet.** [GitHub Releases](../../releases) will host the approved individual mods and the optional collection bundle. GitHub's automatically generated **Source code (zip)** archive is **not** an installable FS25 mod.

## Rights / Rechte

No blanket license is granted for all third-party code, artwork, voices, music or other assets. Permissions, credits and any redistribution limits must be checked for the exact final release payload. Private voice packs and unrelated media must not be included accidentally.

## Feedback / Bugreports

Use [GitHub Issues](../../issues) and include the **exact ZIP SHA-256**, FS25/AutoDrive versions, SP/MP/Dedi context, reproduction steps and a **redacted** current log. Please do not publish personal information, credentials or private server access details.

*Agriculture Science – Automate smarter. Farm better.*
