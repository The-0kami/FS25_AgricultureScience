# Agriculture Science – Farming Simulator 25

**Modulare Automatisierung und Kamera-Werkzeuge für Farming Simulator 25.**  
**Modular automation and camera tools for Farming Simulator 25.**

[Deutsch](#deutsch) · [English](#english) · [Release preparation / Release-Vorbereitung](docs/RELEASE_PREPARATION.md) · [Historische Build-Matrix](docs/BUILD_STATUS.md)

> **Release-Vorbereitung / Release preparation:** Die bereits entwickelten Module werden für eine gemeinsame Veröffentlichung vorbereitet. **Hier ist bislang noch kein installierbares Release veröffentlicht.** Die aktuelle Freigabe, ZIP-Prüfsummen, Mod-Versionen und Tests werden erst anhand der finalen Modarchive festgehalten. Existing October 2026 build notes are historical, not download recommendations.

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

**AutoDrive ist nicht enthalten.** AutoDrive wird für die darauf aufbauenden Fahrabläufe separat benötigt. Je nach Funktion und Modulkombination gelten weitere Bedingungen; die Details werden für das finale Release validiert. Courseplay ist optional, soweit jeweilige Funktionen es unterstützen.

**Spielinterne Tutorials:** Es ist eine Tutorial-/Hilfefunktion vorhanden. Welche Einträge bei Teilinstallationen erscheinen und wie mehrere UI-Versionen zusammenspielen, wird vor dem Release ausdrücklich geprüft. Alte bebilderte Anleitungen sind als historische/ergänzende Dokumentation zu verstehen, nicht als verbindliche Abbildung der aktuellen Oberfläche.

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

**AutoDrive is not bundled.** It is separately required for AutoDrive-based driving features. Feature-specific dependencies and supported module combinations will be validated against the final builds. Courseplay is optional where supported.

**In-game tutorials:** Tutorial/help functionality exists, but module-visibility behavior under partial installations and interactions between differing UI revisions require verification before publication. Older illustrated guides remain historical/supplemental material rather than authoritative depictions of the current UI.

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
