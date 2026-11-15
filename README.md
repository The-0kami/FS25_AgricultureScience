# Agriculture Science
### Modular automation for Farming Simulator 25

**Automate smarter. Farm better.**

Agriculture Science is a collection of independently installable Farming Simulator 25 mods built around smarter vehicle parking, service automation, gate control and cinematic camera workflows.

**[Deutsch](#deutsch) · [English](#english) · [Downloads](#downloads--releases) · [Documentation](#documentation--dokumentation) · [Issues](../../issues)**

> **Release status · In preparation**  
> Three installable modules are being prepared and verified. There is **no public GitHub release yet**. The automatically generated GitHub “Source code” ZIP is **not** an installable FS25 mod.

---

## Deutsch

### Ein Projekt. Mehrere Module.

Agriculture Science erweitert den Landwirtschafts-Simulator 25 um aufeinander abgestimmte Automatisierungswerkzeuge. Installiere die Module, die du benötigst: Jedes der drei geplanten Modpakete bringt seine eigene Menüintegration mit. Für bestimmte gemeinsame Funktionen arbeiten mehrere Module zusammen.

| Modul | Was es macht | Paket |
|:--|:--|:--|
| **A.P.S.** · Advanced Parking Sequence | Unterstützt automatisierte Parkabläufe und Fahrzeugübergaben im Zusammenspiel mit AutoDrive. | Eigenständige Mod |
| **A.S.S.** · Autonomous Service Supervisor | Ergänzt A.P.S. um koordinierte Serviceabläufe für unterstützte Wasch-, Reparatur- und Versorgungsstellen. | **In A.P.S. enthalten** |
| **L.E.G.S.** · Logical Entrance Guidance System | Steuert Tore und unterstützt die Konfiguration von Servicebereichen, Stellplätzen und Interaktionen. | Eigenständige Mod; Dateiname **SmartGate** |
| **N.E.C.K.** · New External Camera Kit | Bietet zusätzliche Kamerafunktionen und Aufnahmemöglichkeiten für AutoDrive-Fahrten. | Eigenständige Mod |

**In Entwicklung:** **H.E.A.D.** – *Heuristic Environmental Analysis Drone*, ein eigenständiges Drohnen- und Scansystem. **Nicht Bestandteil des ersten Downloadpakets.**

### Installation

1. Sichere deinen Spielstand und beende LS25 vollständig.
2. Lade nach Veröffentlichung die gewünschte **Mod-ZIP** von [GitHub Releases](../../releases). A.P.S., L.E.G.S. und N.E.C.K. können einzeln installiert werden.
3. Kopiere die einzelnen Mod-ZIPs **ungeöffnet** in deinen aktiven LS25-Modordner. Ein optionales Agriculture-Science-Komplettpaket muss zuvor entpackt werden.
4. Aktiviere die entsprechenden Mods in deinem Spielstand. Installiere **AutoDrive separat**, wenn du die davon abhängigen Fahrfunktionen verwenden möchtest.

**Zusammenspiel:** A.S.S.-Servicefunktionen benötigen A.P.S. **und** L.E.G.S.; reine L.E.G.S.-Torsteuerung funktioniert eigenständig. N.E.C.K.-Filmfahrten erfordern aktives AutoDrive. Die verwendete AutoDrive-Referenz ist **3.0.1.4**, ohne dass dies eine garantierte Mindestversion darstellt. Courseplay kann optional genutzt werden.

Für Updates, bestehende Serviceplätze und Dedicated Server bitte vorab die Hinweise in der [Installationsdokumentation](docs/de/INSTALLATION.md) und [Kompatibilitätsübersicht](docs/COMPATIBILITY.md) lesen. Einige ältere Anleitungen werden derzeit an den neuen Dreier-Modulstand angepasst.

### Hilfe und Rückmeldungen

Probleme, Verbesserungsvorschläge und Testerfahrungen sind willkommen. Erstelle dafür ein [GitHub Issue](../../issues) mit Modversion, FS25-/AutoDrive-Version, Einzelspieler-/Mehrspieler-/Serverumgebung, Schritten zur Reproduktion und einem **bereinigten** Logauszug. Bitte keine Passwörter, privaten Serverdaten oder persönlichen Informationen veröffentlichen.

---

## English

### One project. Multiple modules.

Agriculture Science extends Farming Simulator 25 with a coordinated set of automation tools. Install only the modules you need: each of the three planned mod packages includes its own menu integration. Some combined features require more than one module.

| Module | What it does | Package |
|:--|:--|:--|
| **A.P.S.** · Advanced Parking Sequence | Supports automated parking sequences and vehicle hand-offs with AutoDrive. | Standalone mod |
| **A.S.S.** · Autonomous Service Supervisor | Adds coordinated service workflows for supported washing, repair and supply facilities. | **Included in A.P.S.** |
| **L.E.G.S.** · Logical Entrance Guidance System | Controls gates and supports service-area, bay and interaction configuration. | Standalone mod; **SmartGate** filename |
| **N.E.C.K.** · New External Camera Kit | Provides additional camera functionality and recording workflows for AutoDrive driving. | Standalone mod |

**In development:** **H.E.A.D.** – *Heuristic Environmental Analysis Drone*, a separate drone and field-scanning system. **Not included in the first download package.**

### Installation

1. Back up your savegame and close FS25.
2. Once available, download the desired **mod ZIP** from [GitHub Releases](../../releases). A.P.S., L.E.G.S. and N.E.C.K. can be installed individually.
3. Copy the individual mod ZIPs **without extracting them** to your active FS25 mods folder. Extract an optional outer Agriculture Science bundle first.
4. Enable the mods for your savegame. Install **AutoDrive separately** for functions that depend on automated driving.

**Integration:** A.S.S. service features require both A.P.S. **and** L.E.G.S.; basic L.E.G.S. gate controls work independently. N.E.C.K. filming drives need active AutoDrive. The development reference for AutoDrive is **3.0.1.4**, not a proven minimum version. Courseplay is optional.

Before upgrading existing installations or configuring a dedicated server, read the [installation guide](docs/en/INSTALLATION.md) and [compatibility notes](docs/COMPATIBILITY.md). Some older guides are being revised for the three-module package.

### Support and feedback

Bug reports, suggestions and external testing feedback are welcome through [GitHub Issues](../../issues). Include mod version, FS25/AutoDrive versions, SP/MP/dedicated-server context, steps to reproduce and a **redacted** log. Do not post credentials, private server details or personal data.

---

## Downloads / Releases

**Preparing the first GitHub release.** The planned downloads are:

- `FS25_APS_AgricultureScience.zip` — A.P.S. **including A.S.S.**
- `FS25_SmartGate_AgricultureScience.zip` — L.E.G.S.
- `FS25_NECK_AgricultureScience.zip` — N.E.C.K.
- An optional **Complete** archive containing the same three individual ZIPs (extract this outer archive before installing).

**[GitHub Releases](../../releases)** is the intended download location. **No installable assets have been published yet.** H.E.A.D. and internal DevTools are excluded.

## Documentation / Dokumentation

| Deutsch | English |
|:--|:--|
| [Installation](docs/de/INSTALLATION.md) | [Installation](docs/en/INSTALLATION.md) |
| [A.P.S. Tutorial](docs/de/TUTORIAL_APS.md) | [A.P.S. Tutorial](docs/en/TUTORIAL_APS.md) |
| [A.S.S. Tutorial](docs/de/TUTORIAL_ASS.md) | [A.S.S. Tutorial](docs/en/TUTORIAL_ASS.md) |
| [L.E.G.S. Tutorial](docs/de/TUTORIAL_LEGS.md) | [L.E.G.S. Tutorial](docs/en/TUTORIAL_LEGS.md) |
| [Fehlerdiagnose](docs/de/TROUBLESHOOTING.md) | [Troubleshooting](docs/en/TROUBLESHOOTING.md) |

[Compatibility / Kompatibilität](docs/COMPATIBILITY.md) · [Known issues / Bekannte Einschränkungen](docs/KNOWN_ISSUES.md) · [Changelog](CHANGELOG.md) · [Release preparation (technical)](docs/RELEASE_PREPARATION.md) · [Historical builds](docs/BUILD_STATUS.md)

## Credits & rights / Rechte

Agriculture Science is an independent community mod project for Farming Simulator 25. AutoDrive and Courseplay are separate projects and are not bundled here. Rights for any included third-party code, audio, artwork and other assets must be verified for each final release; this repository does not grant a blanket license to third-party materials.

---

*Agriculture Science · Automate smarter. Farm better.*
