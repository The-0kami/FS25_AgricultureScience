# Agriculture Science – Release preparation / Release-Vorbereitung

> **Planning document / Planungsdokument, 14 November 2026; user-confirmed local status.** Not an announcement of a published release, a passed GIANTS test or a confirmed ModHub submission. The October candidate hashes in [BUILD_STATUS.md](BUILD_STATUS.md) remain **historical**.

## Deutsch

### Release-Aufbau

**Ein GitHub-Repository und ein zentraler GitHub-Release pro freigegebener Paketgeneration.** Es gibt drei installierbare, separat nutzbare Mod-ZIPs:

1. `FS25_APS_AgricultureScience.zip` – A.P.S. einschließlich A.S.S.
2. `FS25_SmartGate_AgricultureScience.zip` – L.E.G.S. (technische SmartGate-Mod-ID)
3. `FS25_NECK_AgricultureScience.zip` – N.E.C.K.

Die lokal gemeldeten Dateinamen und Versionen sind unten erfasst; sie müssen beim Eingang der finalen ZIPs erneut kontrolliert werden. **H.E.A.D. ist zunächst nur als „In Development“ erwähnt**, nicht im ersten Release; DevTools und private Audio-Pakete werden nicht verteilt.

Dazu kann ein äußeres Archiv `AgricultureScience_Complete_<release>.zip` erscheinen, dessen Inhalt aus **genau denselben unveränderten drei installierbaren ZIPs** besteht. Das äußere Archiv selbst wird **nicht** in LS25 als Mod installiert. Ein Release muss eine Liste der enthaltenen Modulversionen und **SHA-256 jedes Archivs** enthalten.

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

### Offene Prüfungen vor Veröffentlichung

- [ ] Die drei **aktuellen, freigegebenen Original-Mod-ZIPs** liegen tatsächlich vor; Dateinamen, ZIP-Test/CRC, Verzeichnisstruktur, `modDesc.xml`, Mod-ID und Version sind geprüft.
- [ ] Keine Duplikate/alten Fassungen/Privatpakete in den Releases; A.S.S. wird nicht fälschlich als eigene Mod-ZIP geführt.
- [ ] Testmatrix mit **A.P.S. allein**, **L.E.G.S. allein**, **N.E.C.K. allein**, **A.P.S.+L.E.G.S.** und **allen drei gemeinsam**. Abhängigkeiten und nur teilweise verfügbare Funktionen korrekt erklären.
- [x] Vom Nutzer gemeldete Lua-Tests: Teilinstallationen, fehlende/inkompatible Tourdaten, Modultext-Austausch bei gleichem Host bestanden (keine unabhängige Prüfung in dieser Dokumentationsarbeit).
- [ ] Modulare Tour im Spiel prüfen: Registrierung, tatsächliche Menüposition, ausgegraute fehlende Module, Deep-Dive-Überspringen, entfernte Mods, unterschiedliche UI-/Host-Versionen und DE/EN-Fallback.
- [ ] Neueste L.E.G.S.-Effekte, Weltmarkierungen, Kraftfeld und lokale Kartenfarben im Spiel prüfen.
- [ ] H.E.A.D.-Sichtprüfung separat im Entwicklungsprojekt; kein Freigabekandidat des Dreierpakets.
- [ ] Erstinstallation und Upgradepfad mit Sicherungen; wichtige Migrationen aus älteren SmartGate-/AD-Zielen dokumentiert.
- [ ] SP/MP/Dedi-Testumfang auf Basis der finalen ZIPs dokumentiert; ungetestete Fälle als solche ausweisen.
- [ ] Rechte und Weitergabe für **alle tatsächlich enthaltenen** Sounds, Stimmen, Bilder, Code und Modelle dokumentiert; keine fremden privaten Assets einpacken.
- [ ] Dokumentation, bekannte Einschränkungen, Changelog, Release Notes und Hashes auf exakt denselben Stand bringen.
- [ ] **Freigabe des Projektinhabers**, erst danach Tag/öffentlicher Release/weitere Plattformen.

### Dokumentationsprinzip

Die bisherige Bildgalerie bleibt als dokumentierte ältere UI-Illustration erhalten. Sie ist **keine** Garantie, dass die abgebildeten Menüs noch dem fertigen Build entsprechen. Spielinterne Tutorials sollen die primäre Bedienhilfe sein, **sofern** ihre Verfügbarkeit unter den gewählten Modulkonstellationen bestätigt wurde. Die README bleibt für die Installation und den Einstieg unverzichtbar.

### Update-Regel

Ein neuer zentraler Release bekommt eine eigene Paketkennung und dokumentiert **pro Modul** dessen unveränderte interne Versionsnummer. Ein Update an einem Modul erzwingt keine künstliche Versionssteigerung der anderen. Kein Vermischen von unveröffentlichten Entwicklungs-ZIPs mit einem freigegebenen Paket.

## English

### Release layout

**One GitHub repository and one central GitHub Release per approved package generation.** Three independently installable ZIP files are planned: A.P.S. (including A.S.S.), L.E.G.S. (technical SmartGate mod ID) and N.E.C.K. Locally reported filenames and versions are recorded below and must be rechecked against the final submitted archives. H.E.A.D. is **in development**, not in the initial release; DevTools and private audio are excluded.

An optional outer `AgricultureScience_Complete_<release>.zip` contains **exactly the same unchanged individual mod ZIPs**. Extract this outer bundle first; **do not** install it as a game mod. Publish module versions and SHA-256 hashes for each archive.

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

### Pre-release checks

- [ ] Receive and verify the **actual approved current mod archives** (ZIP/CRC, structure, `modDesc.xml`, mod IDs and versions).
- [ ] Keep A.S.S. within A.P.S.; exclude duplicate versions, DevTools and private packs.
- [ ] Test each module alone, A.P.S.+L.E.G.S., and the full combination; document dependencies accurately.
- [x] Record user-reported passing Lua tests: partial installations, missing/incompatible tour data, and module-text replacement with the same host (not independently verified in this documentation task).
- [ ] Verify the modular tour in game: registration, actual menu location, greyed-out missing modules, Deep Dive skipping, removed mods, differing UI/host revisions and DE/EN fallback.
- [ ] Verify the latest L.E.G.S. effects, world markers, force field and local map colours in game.
- [ ] Track H.E.A.D. visual testing separately in development; it is not a candidate for the three-mod package.
- [ ] Verify fresh installation, upgrades and any SmartGate/AutoDrive target migration.
- [ ] Record actually verified SP/MP/Dedi scenarios and clearly state unverified scenarios.
- [ ] Audit redistribution rights for the exact shipped code, media and assets.
- [ ] Align README, changelog, known limitations, release notes and checksums with the **same** release payload.
- [ ] Obtain explicit owner approval before publishing a tag, release or ModHub submission.

### Documentation and update policy

The existing illustration catalogue is historical/supplemental, not proof of the current UI. Embedded tutorials can become the primary usage guide **after** their module-combination behavior is verified. Each central release records the actual version of each module; changing one module does not require a fake version increment for unchanged modules. No development candidate should be silently substituted for a released archive.
