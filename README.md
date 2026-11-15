# Agriculture Science – Farming Simulator 25

**Modulare Automatisierung und Kamera-Werkzeuge für Farming Simulator 25.**  
**Modular automation and camera tools for Farming Simulator 25.**

[Deutsch](#deutsch) · [English](#english) · [Release preparation / Release-Vorbereitung](docs/RELEASE_PREPARATION.md) · [Historische Build-Matrix](docs/BUILD_STATUS.md)

> **Release-Vorbereitung / Release preparation – 15.11.2026:** Lokaler Stand vom Nutzer bestätigt; **keine Release-Freigabe**. Local versions and candidate SHA-256 hashes are documented below; they are **not approved downloads**. October 2026 build notes remain historical.

## Deutsch

Agriculture Science besteht aus **unabhängig installierbaren Modulen**. Jedes Modul bringt laut aktuellem Projektstand seine eigene Menü-/UI-Integration mit. Es ist keine zusätzliche gemeinsame GUI-Mod vorgesehen.

| Modul | Zweck | Verteilung |
|---|---|---|
| **A.P.S. – Advanced Parking Sequence** | Koordiniert AutoDrive-Parkabläufe und unterstützte Geräte-/Fahrzeugübergaben | Eigenständige Mod-ZIP |
| **A.S.S. – Autonomous Service Supervisor** | Koordiniert unterstützte Wasch-, Reparatur-, Tank-/Ladeabläufe und Serviceanzeigen | **Bestandteil von A.P.S.**, keine eigene ZIP |
| **L.E.G.S. – Logical Entrance Guidance System** | Tore, Interaktionen und Infrastruktur für Servicebereiche, Bays und Reservierungen | Eigenständige Mod-ZIP mit technischer SmartGate-Identität |
| **N.E.C.K. – New External Camera Kit** | Eigenständige Kameramod mit Kameraperspektiven und Aufnahmen im AutoDrive-Fahrkontext | Eigenständige Mod-ZIP |
| **H.E.A.D. – Heuristic Environmental Analysis Drone** | Separate Drohnen-/Scan-Mod, derzeit in Entwicklung | **Nicht Teil des ersten Releases** |

**Geplante Downloads (noch nicht veröffentlicht; ZIPs liegen nur lokal vor):** Einzel-ZIPs für A.P.S. (inkl. A.S.S.), L.E.G.S. und N.E.C.K.; zusätzlich ein **Komplettpaket**, das dieselben unveränderten Mod-ZIPs enthält. Das Komplettpaket muss vor der Installation **entpackt** werden; nur die einzelnen installierbaren Mod-ZIPs gehören in den aktiven Mods-Ordner.

### Maßgeblicher gebündelter BB-Export – 15.11.2026 (nur lokal)

Vom Projektinhaber gemeldeter lokaler Export: `Build_Exports/AgricultureScience_BB_Export_20261115.zip` mit **gemeldeter** SHA-256 `26b5879bd0d57ec0921f5b284d2aecbaff01ab30b9c2eff384ad2df924cf3a26`.

Laut Übergabe enthält das Archiv die aktuellen drei Mod-ZIPs (A.P.S. einschließlich A.S.S., L.E.G.S., N.E.C.K.), das **separate NECK BeatSync Tool** sowie UI-/GUI-Vorschauen und Mod-Bilder. H.E.A.D. und DevTools sind ausgeschlossen. **Das BeatSync Tool ist keine vierte FS25-Mod-ZIP**; seine Handhabung und Weitergabefreigabe müssen nach Einsicht in die tatsächlichen Dateien getrennt dokumentiert werden. Der BB-Export ist ein lokales Übergabe-/Arbeitsarchiv und **kein veröffentlichtes oder direkt in LS25 zu installierendes Modpaket**.

**Status:** Der lokale Windows-Pfad ist von dieser Umgebung aus nicht zugänglich. Weder das Archiv noch innere Dateien sind hier eingegangen. Deshalb sind Inhaltsliste, BB-Hash und die Übereinstimmung der inneren Mod-ZIPs mit den unten dokumentierten **zuvor gemeldeten Einzelarchiv-Hashes** noch nicht unabhängig bestätigt. Die BB-Export-Dateien gelten als maßgebliche Release-Kandidaten; bei Abweichungen müssen die inneren Hashes nach Eingang neu dokumentiert werden.

**Neue Pflichtabhängigkeiten laut aktuellem Build:** A.P.S. und N.E.C.K. deklarieren in `modDesc.xml` jeweils `FS25_AutoDrive` als Pflichtmod. Der Nutzer berichtet, dass LS25 beim Aktivieren dieser Mods AutoDrive automatisch zur Auswahl angeboten hat. Dies ist ein berichteter Ingame-Test, keine hier eigenständig ausgelesene `modDesc.xml`. L.E.G.S. ist eigenständig nutzbar, mit optionalen AutoDrive-Funktionen.

### Zuvor gemeldete Einzel-ZIP-Kandidaten – 15.11.2026

Vom Projektinhaber gemeldete aktuellere ZIP-Exporte im lokalen Ordner `Build_Exports/`; CRC, `modDesc.xml` und gemeinsamer Settings-Host wurden nach dessen Angaben lokal geprüft. **Diese Archivdateien wurden hier nicht empfangen und ihre SHA-256 nicht unabhängig nachgerechnet. Keine GitHub-Uploads und keine freigegebenen Downloads.** Die Hashes vom 14.11.2026 sind überholt.

| Modul / Module | Version | ZIP | SHA-256 |
|---|---|---|---|
| A.P.S. (inkl. A.S.S. und Audio / incl. A.S.S. and audio) | 1.0.0.0 | `FS25_APS_AgricultureScience.zip` | `e543cc3cde6e1f7511dc889861932e4f79cab49b4a603b977370f123138fdf66` |
| L.E.G.S. | 1.0.0.0 | `FS25_SmartGate_AgricultureScience.zip` | `7aa228b254fd149f4b4f9c3483788de9e7a506e526109424210e745e3514cdbb` |
| N.E.C.K. | 0.1.0.0 | `FS25_NECK_AgricultureScience.zip` | `c599e496e3d6571a2adf981d493490abecdfdc3bfbfc78e759ee41177df1366b` |

**Abhängigkeiten:** A.P.S. und N.E.C.K. deklarieren laut aktuellem Build `FS25_AutoDrive` als **Pflichtmod**. LS25 bot bei der Mod-Auswahl laut Nutzertest die automatische Mit-Auswahl an. AutoDrive **3.0.1.4** ist die verwendete Referenz, keine daraus abgeleitete Mindestversion. AutoDrive muss verfügbar und aktiviert sein. N.E.C.K.-Filmfahrten benötigen aktives AutoDrive; die Vorschau funktioniert im besetzten Fahrzeug ohne aktives AutoDrive. L.E.G.S.-Torsteuerung läuft eigenständig; AutoDrive-Voröffnung ist optional. Die A.S.S.-Ansicht setzt geladenes A.P.S.+L.E.G.S. und eine registrierte Ansicht voraus.

**Tutorials und Host:** Alle drei Mods enthalten den gemeinsamen Host; der Host-Umbau erfolgte einmalig und koordiniert. Tourtexte und Gruppen stammen jetzt aus den Einstellungsmodulen. Fehlende Module sind ausgegraut und werden im Deep Dive übersprungen. Laut Nutzer bestanden die Lua-Tests für Teilinstallationen, fehlende/inkompatible Tourdaten und den Austausch eines Modultexts bei gleichem Host. Die modulare Tour muss noch im Spiel geprüft werden.

**L.E.G.S. neu:** „Serviceplätze → Beispiel“ erklärt einen Bereich gegenüber zwei Bays. Quelle und AD-Haltepunkt werden direkt in der Welt dargestellt; eigenes Kraftfeld und lokale Farben erscheinen auf den L.E.G.S./A.S.S.-Karten. Die neuesten Effekte sind noch im Spiel zu prüfen.

**Separat in Entwicklung:** H.E.A.D. **0.1.0.0** mit 6,9 Sekunden Startanimation, neuem räumlichem Scan, Ergebnisbox am Feld und bis zu acht überlappenden Scanflächen pro Flug; visueller Ingame-Test offen. DevTools **0.5.0.0** ist ein internes Diagnosewerkzeug. Beide gehören nicht ins öffentliche Dreierpaket.

**BB-Export:** Das maßgebliche lokale Übergabearchiv umfasst laut Projektinhaber auch das separate N.E.C.K. BeatSync Tool und weitere UI-/GUI-Vorschauen; eine Sichtung und Freigabe zur separaten Verteilung stehen aus.

**Bilder für die Projektseite:** Drei Modul-Icons (APS, LEGS, NECK; je 512×512) und ein echter Servicebereich-Screenshot sind lokal als `AgricultureScience_GitHub_Bilder_20261115.zip` vorbereitet. **Noch nicht hochgeladen oder hier visuell geprüft.** Weitere Zuordnung: [Release-Vorbereitung](docs/RELEASE_PREPARATION.md).

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

**Planned downloads (not published yet; ZIPs currently available locally only):** Individual ZIP files for A.P.S. (including A.S.S.), L.E.G.S. and N.E.C.K., plus a **Complete Package** containing those same unmodified ZIP files. Extract the outer Complete Package first; install only the individual mod ZIPs into the active mods directory.

### Authoritative bundled BB export – 15 November 2026 (local only)

Owner-reported local export: `Build_Exports/AgricultureScience_BB_Export_20261115.zip`, **reported** SHA-256 `26b5879bd0d57ec0921f5b284d2aecbaff01ab30b9c2eff384ad2df924cf3a26`.

The export reportedly contains the three current FS25 mod ZIPs (A.P.S. including A.S.S., L.E.G.S., N.E.C.K.), the **separate NECK BeatSync tool**, plus UI/GUI previews and mod artwork. H.E.A.D. and DevTools are excluded. **BeatSync is not a fourth installable FS25 mod ZIP**; its packaging, instructions and redistribution approval need separate review after receiving the files. The BB export is a local handoff/work archive, **not a published or directly installable game mod package**.

**Verification status:** The Windows path cannot be accessed from this environment. Neither the bundle nor its contained files has been received. Its manifest, bundle SHA-256, and whether its inner mod ZIPs match the **previously reported individual ZIP SHA-256 values below** therefore remain unverified. Use the BB export as the authoritative candidate source; replace individual hashes if verification shows that its contents differ.

**New declared dependencies (owner report):** Both A.P.S. and N.E.C.K. now declare `FS25_AutoDrive` as a required mod in `modDesc.xml`. The owner reports that LS25 offered to automatically select AutoDrive when enabling the mods. This is a reported in-game test, not a `modDesc.xml` inspection performed here. L.E.G.S. remains independently usable, with optional AutoDrive integration.

### Previously reported individual ZIP candidates – 15 November 2026

Newer ZIP exports reported by the project owner in the local `Build_Exports/` directory; CRC, `modDesc.xml` and shared settings host were reportedly checked locally. **The archives have not been received here and their SHA-256 values have not been independently recalculated. No GitHub uploads or approved downloads.** The 14 November checksums are superseded.

| Modul / Module | Version | ZIP | SHA-256 |
|---|---|---|---|
| A.P.S. (inkl. A.S.S. und Audio / incl. A.S.S. and audio) | 1.0.0.0 | `FS25_APS_AgricultureScience.zip` | `e543cc3cde6e1f7511dc889861932e4f79cab49b4a603b977370f123138fdf66` |
| L.E.G.S. | 1.0.0.0 | `FS25_SmartGate_AgricultureScience.zip` | `7aa228b254fd149f4b4f9c3483788de9e7a506e526109424210e745e3514cdbb` |
| N.E.C.K. | 0.1.0.0 | `FS25_NECK_AgricultureScience.zip` | `c599e496e3d6571a2adf981d493490abecdfdc3bfbfc78e759ee41177df1366b` |

**Dependencies:** A.P.S. and N.E.C.K. now reportedly declare `FS25_AutoDrive` as a **required mod**. During mod selection, LS25 reportedly offered to automatically select AutoDrive. AutoDrive **3.0.1.4** is the reference used, not an inferred minimum version. AutoDrive must be available and enabled. N.E.C.K. filming drives require active AutoDrive; preview works in an occupied vehicle without active AutoDrive. L.E.G.S. gate control works independently; AutoDrive pre-opening is optional. The A.S.S. view requires loaded A.P.S.+L.E.G.S. and a registered view.

**Tutorials and host:** All three mods carry the shared host; its refactoring was a single coordinated change. Tour text and groups now come from the settings modules. Missing modules are greyed out and skipped by Deep Dive. The user reports passing Lua tests for partial installations, missing/incompatible tour data, and replacing a module text while retaining the same host. The modular tour still needs in-game verification.

**New in L.E.G.S.:** “Service spaces → Example” explains one area versus two bays. The source and AD stopping point are shown directly in the world; a dedicated force field and local colours appear on the L.E.G.S./A.S.S. maps. The latest effects still need in-game verification.

**Separate development:** H.E.A.D. **0.1.0.0** has a 6.9-second start animation, a new spatial scan, a result box at the field, and up to eight overlapping scan areas per flight; visual in-game testing is pending. DevTools **0.5.0.0** is an internal diagnostic tool. Neither belongs in the public three-mod package.

**BB export:** The authoritative local handoff bundle reportedly also includes the separate N.E.C.K. BeatSync tool and further UI/GUI previews; inspection and separate redistribution approval remain pending.

**Images for the project page:** Three 512×512 module icons (APS, LEGS, NECK) and one in-game service-area screenshot are reportedly bundled locally as `AgricultureScience_GitHub_Bilder_20261115.zip`. **Not uploaded or visually inspected here yet.** See [release preparation](docs/RELEASE_PREPARATION.md).

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
