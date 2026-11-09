# Agriculture Science – Release preparation / Release-Vorbereitung

> **Planning document / Planungsdokument, 9 November 2026.** Not an announcement of a published release, a passed GIANTS test or a confirmed ModHub submission. The October candidate hashes in [BUILD_STATUS.md](BUILD_STATUS.md) remain **historical**.

## Deutsch

### Release-Aufbau

**Ein GitHub-Repository und ein zentraler GitHub-Release pro freigegebener Paketgeneration.** Es gibt drei installierbare, separat nutzbare Mod-ZIPs:

1. `FS25_APS_AgricultureScience.zip` – A.P.S. einschließlich A.S.S.
2. `FS25_SmartGate_AgricultureScience.zip` – L.E.G.S. (technische SmartGate-Mod-ID)
3. `FS25_NECK_AgricultureScience.zip` – N.E.C.K.

Die tatsächlichen Dateinamen und enthaltenen Versionen werden beim Eingang der finalen ZIPs kontrolliert. **H.E.A.D. ist zunächst nur als „In Development“ erwähnt**, nicht im ersten Release; DevTools und private Audio-Pakete werden nicht verteilt.

Dazu kann ein äußeres Archiv `AgricultureScience_Complete_<release>.zip` erscheinen, dessen Inhalt aus **genau denselben unveränderten drei installierbaren ZIPs** besteht. Das äußere Archiv selbst wird **nicht** in LS25 als Mod installiert. Ein Release muss eine Liste der enthaltenen Modulversionen und **SHA-256 jedes Archivs** enthalten.

### Offene Prüfungen vor Veröffentlichung

- [ ] Die drei **aktuellen, freigegebenen Original-Mod-ZIPs** liegen tatsächlich vor; Dateinamen, ZIP-Test/CRC, Verzeichnisstruktur, `modDesc.xml`, Mod-ID und Version sind geprüft.
- [ ] Keine Duplikate/alten Fassungen/Privatpakete in den Releases; A.S.S. wird nicht fälschlich als eigene Mod-ZIP geführt.
- [ ] Testmatrix mit **A.P.S. allein**, **L.E.G.S. allein**, **N.E.C.K. allein**, **A.P.S.+L.E.G.S.** und **allen drei gemeinsam**. Abhängigkeiten und nur teilweise verfügbare Funktionen korrekt erklären.
- [ ] **Codex bestätigt Tutorial-Registrierung und Host-Verhalten**: Teilinstallation, entfernte Mods, unterschiedliche mitgelieferte UI-Versionen, DE/EN-Fallback und tatsächliche Menüposition.
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

**One GitHub repository and one central GitHub Release per approved package generation.** Three independently installable ZIP files are planned: A.P.S. (including A.S.S.), L.E.G.S. (technical SmartGate mod ID) and N.E.C.K. Final filenames and versions must be checked against the submitted archives. H.E.A.D. is **in development**, not in the initial release; DevTools and private audio are excluded.

An optional outer `AgricultureScience_Complete_<release>.zip` contains **exactly the same unchanged individual mod ZIPs**. Extract this outer bundle first; **do not** install it as a game mod. Publish module versions and SHA-256 hashes for each archive.

### Pre-release checks

- [ ] Receive and verify the **actual approved current mod archives** (ZIP/CRC, structure, `modDesc.xml`, mod IDs and versions).
- [ ] Keep A.S.S. within A.P.S.; exclude duplicate versions, DevTools and private packs.
- [ ] Test each module alone, A.P.S.+L.E.G.S., and the full combination; document dependencies accurately.
- [ ] Obtain Codex confirmation of **in-game tutorial location and registration**, behavior when modules are absent, different bundled UI revisions and DE/EN fallback.
- [ ] Verify fresh installation, upgrades and any SmartGate/AutoDrive target migration.
- [ ] Record actually verified SP/MP/Dedi scenarios and clearly state unverified scenarios.
- [ ] Audit redistribution rights for the exact shipped code, media and assets.
- [ ] Align README, changelog, known limitations, release notes and checksums with the **same** release payload.
- [ ] Obtain explicit owner approval before publishing a tag, release or ModHub submission.

### Documentation and update policy

The existing illustration catalogue is historical/supplemental, not proof of the current UI. Embedded tutorials can become the primary usage guide **after** their module-combination behavior is verified. Each central release records the actual version of each module; changing one module does not require a fake version increment for unchanged modules. No development candidate should be silently substituted for a released archive.
