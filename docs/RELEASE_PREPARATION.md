# Agriculture Science – Release preparation / Release-Vorbereitung

> **Planning document / Planungsdokument, 15 November 2026; owner-reported local export candidate status.** Not an announcement of a published release, a passed GIANTS test or a confirmed ModHub submission. The October candidate hashes in [BUILD_STATUS.md](BUILD_STATUS.md) remain **historical**.

## Deutsch

### Release-Aufbau

**Ein GitHub-Repository und ein zentraler GitHub-Release pro freigegebener Paketgeneration.** Es gibt drei installierbare, separat nutzbare Mod-ZIPs:

1. `FS25_APS_AgricultureScience.zip` – A.P.S. einschließlich A.S.S.
2. `FS25_SmartGate_AgricultureScience.zip` – L.E.G.S. (technische SmartGate-Mod-ID)
3. `FS25_NECK_AgricultureScience.zip` – N.E.C.K.

Die lokal gemeldeten Dateinamen und Versionen sind unten erfasst; sie müssen beim Eingang der finalen ZIPs erneut kontrolliert werden. **H.E.A.D. ist zunächst nur als „In Development“ erwähnt**, nicht im ersten Release; DevTools und private Audio-Pakete werden nicht verteilt.

Dazu kann ein äußeres Archiv `AgricultureScience_Complete_<release>.zip` erscheinen, dessen Inhalt aus **genau denselben unveränderten drei installierbaren ZIPs** besteht. Das äußere Archiv selbst wird **nicht** in LS25 als Mod installiert. Ein Release muss eine Liste der enthaltenen Modulversionen und **SHA-256 jedes Archivs** enthalten.

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

**Abhängigkeiten:** A.P.S. und N.E.C.K. deklarieren laut aktuellem Build `FS25_AutoDrive` als **Pflichtmod**; beim Aktivieren bot LS25 nach Nutzertest die automatische AutoDrive-Mit-Auswahl an. AutoDrive **3.0.1.4** ist eine Referenz, keine festgelegte Mindestversion. AutoDrive muss installiert und aktiviert sein. N.E.C.K.-Filmfahrten benötigen aktives AutoDrive; die Vorschau funktioniert im besetzten Fahrzeug ohne aktives AutoDrive. L.E.G.S.-Torsteuerung läuft eigenständig; AutoDrive-Voröffnung ist optional. Die A.S.S.-Ansicht setzt geladenes A.P.S.+L.E.G.S. und eine registrierte Ansicht voraus.

**Tutorials und Host:** Alle drei Mods enthalten den gemeinsamen Host; der Host-Umbau erfolgte einmalig und koordiniert. Tourtexte und Gruppen stammen jetzt aus den Einstellungsmodulen. Fehlende Module sind ausgegraut und werden im Deep Dive übersprungen. Laut Nutzer bestanden die Lua-Tests für Teilinstallationen, fehlende/inkompatible Tourdaten und den Austausch eines Modultexts bei gleichem Host. Die modulare Tour muss noch im Spiel geprüft werden.

**L.E.G.S. neu:** „Serviceplätze → Beispiel“ erklärt einen Bereich gegenüber zwei Bays. Quelle und AD-Haltepunkt werden direkt in der Welt dargestellt; eigenes Kraftfeld und lokale Farben erscheinen auf den L.E.G.S./A.S.S.-Karten. Die neuesten Effekte sind noch im Spiel zu prüfen.

**Separat in Entwicklung:** H.E.A.D. **0.1.0.0** mit 6,9 Sekunden Startanimation, neuem räumlichem Scan, Ergebnisbox am Feld und bis zu acht überlappenden Scanflächen pro Flug; visueller Ingame-Test offen. DevTools **0.5.0.0** ist ein internes Diagnosewerkzeug. Beide gehören nicht ins öffentliche Dreierpaket.

### Vorgesehene GitHub-Bilder – lokale Dateien, noch nicht hochgeladen

Der Projektinhaber meldet vier lokal exportierte Dateien im Archiv `AgricultureScience_GitHub_Bilder_20261115.zip`. **Es wurden noch keine Bilddateien ins Repository oder in einen GitHub-Release hochgeladen; Sichtprüfung und Bild-Hashes stehen aus.**

- `aps-mod-icon.png`, `legs-mod-icon.png`, `neck-mod-icon.png`: jeweils gemeldete 512×512-PNG-Exporte aus den im `modDesc.xml` der aktuellen Mod-ZIPs referenzierten Icons. Nach Erhalt als kleine Modulübersicht in der README vorgesehen.
- `ass-servicebereich-ingame.png`: gemeldeter echter Ingame-Screenshot mit cyanfarbener Bereichsbegrenzung und AD-Zielpfeil. Als Funktionsvorschau in der README und als Ergänzung in `docs/de/TUTORIAL_LEGS.md`, `docs/en/TUTORIAL_LEGS.md`, `docs/de/TUTORIAL_ASS.md` und `docs/en/TUTORIAL_ASS.md` vorgesehen; Bildinhalt zunächst gegen Build und Sprachfassung prüfen.

Vorgesehener Repository-Zielordner nach Sichtprüfung: `docs/assets/release/20261115/`. Vorhandene historische UI-Illustrationen in `docs/assets/ui/` nicht kommentarlos überschreiben.

### Offene Prüfungen vor Veröffentlichung

- [ ] Maßgeblichen **BB-Export** tatsächlich empfangen, SHA-256 `26b5879bd0d57ec0921f5b284d2aecbaff01ab30b9c2eff384ad2df924cf3a26` nachrechnen, Inhaltsliste prüfen (drei Mods, BeatSync, Medien; keine HEAD/DevTools); innere ZIP-Hashes mit den bisher gemeldeten Einzelwerten vergleichen.
- [ ] Drei gemeldete **aktuelle Original-Mod-ZIPs** tatsächlich empfangen; CRC, Struktur, `modDesc.xml`, Mod-ID, Version und SHA-256 **unabhängig** prüfen und mit den gemeldeten Export-Hashes vergleichen.
- [ ] `FS25_AutoDrive` als Pflichtabhängigkeit für A.P.S./N.E.C.K. in den tatsächlichen `modDesc.xml` prüfen und Ingame-Mit-Auswahl sowie fehlendes AutoDrive testen; L.E.G.S. ohne AD prüfen.
- [ ] BeatSync-Tool separat sichten, Lizenz/Verteilrechte, Nutzungsanleitung und geeignete Auslieferung bestimmen; nicht stillschweigend als vierte Mod-ZIP behandeln.
- [ ] Keine Duplikate/alten Fassungen/Privatpakete in den Releases; A.S.S. wird nicht fälschlich als eigene Mod-ZIP geführt.
- [ ] Testmatrix mit **A.P.S. allein**, **L.E.G.S. allein**, **N.E.C.K. allein**, **A.P.S.+L.E.G.S.** und **allen drei gemeinsam**. Abhängigkeiten und nur teilweise verfügbare Funktionen korrekt erklären.
- [x] Vom Nutzer gemeldete Lua-Tests: Teilinstallationen, fehlende/inkompatible Tourdaten, Modultext-Austausch bei gleichem Host bestanden (keine unabhängige Prüfung in dieser Dokumentationsarbeit).
- [ ] Modulare Tour im Spiel prüfen: Registrierung, tatsächliche Menüposition, ausgegraute fehlende Module, Deep-Dive-Überspringen, entfernte Mods, unterschiedliche UI-/Host-Versionen und DE/EN-Fallback.
- [ ] Neueste L.E.G.S.-Effekte, Weltmarkierungen, Kraftfeld und lokale Kartenfarben im Spiel prüfen.
- [ ] H.E.A.D.-Sichtprüfung separat im Entwicklungsprojekt; kein Freigabekandidat des Dreierpakets.
- [ ] Erstinstallation und Upgradepfad mit Sicherungen; wichtige Migrationen aus älteren SmartGate-/AD-Zielen dokumentiert.
- [ ] SP/MP/Dedi-Testumfang auf Basis der finalen ZIPs dokumentiert; ungetestete Fälle als solche ausweisen.
- [ ] Rechte und Weitergabe für **alle tatsächlich enthaltenen** Sounds, Stimmen, Bilder, Code und Modelle dokumentiert; keine fremden privaten Assets einpacken.
- [ ] Vier neue GitHub-PNGs tatsächlich empfangen, ansehen, Rechte/Herkunft sowie Hashes prüfen und erst dann in README und Doku einbinden.
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

**Dependencies:** A.P.S. and N.E.C.K. reportedly declare `FS25_AutoDrive` as a **required mod**; LS25 offered to auto-select AutoDrive in the owner's test. AutoDrive **3.0.1.4** is a reference, not an established minimum version. AutoDrive must be installed and enabled. N.E.C.K. filming drives require active AutoDrive; preview works in an occupied vehicle without active AutoDrive. L.E.G.S. gate control works independently; AutoDrive pre-opening is optional. The A.S.S. view requires loaded A.P.S.+L.E.G.S. and a registered view.

**Tutorials and host:** All three mods carry the shared host; its refactoring was a single coordinated change. Tour text and groups now come from the settings modules. Missing modules are greyed out and skipped by Deep Dive. The user reports passing Lua tests for partial installations, missing/incompatible tour data, and replacing a module text while retaining the same host. The modular tour still needs in-game verification.

**New in L.E.G.S.:** “Service spaces → Example” explains one area versus two bays. The source and AD stopping point are shown directly in the world; a dedicated force field and local colours appear on the L.E.G.S./A.S.S. maps. The latest effects still need in-game verification.

**Separate development:** H.E.A.D. **0.1.0.0** has a 6.9-second start animation, a new spatial scan, a result box at the field, and up to eight overlapping scan areas per flight; visual in-game testing is pending. DevTools **0.5.0.0** is an internal diagnostic tool. Neither belongs in the public three-mod package.

### Proposed GitHub images – local only, not uploaded

The project owner reports four locally exported files in `AgricultureScience_GitHub_Bilder_20261115.zip`. **No image files have been uploaded to the repository or a GitHub Release; visual inspection and image checksums remain pending.**

- `aps-mod-icon.png`, `legs-mod-icon.png`, `neck-mod-icon.png`: reported 512×512 PNG exports of the icons referenced by the current mod ZIPs' `modDesc.xml`; intended as a compact module overview in README after delivery.
- `ass-servicebereich-ingame.png`: reported actual in-game screenshot showing a cyan service-area boundary and AD destination arrow. Intended for the README feature preview and `docs/de/TUTORIAL_LEGS.md`, `docs/en/TUTORIAL_LEGS.md`, `docs/de/TUTORIAL_ASS.md`, `docs/en/TUTORIAL_ASS.md` after image/build/language review.

Proposed repository destination after inspection: `docs/assets/release/20261115/`. Do not silently overwrite historical illustrations in `docs/assets/ui/`.

### Pre-release checks

- [ ] Receive the **authoritative BB bundle**, recalculate its reported SHA-256 `26b5879bd0d57ec0921f5b284d2aecbaff01ab30b9c2eff384ad2df924cf3a26`, inspect the actual contents (three mods, BeatSync, media, no HEAD/DevTools) and compare inner ZIP hashes against the previously reported individual values.
- [ ] Receive the three **actual current mod archives**; independently verify CRC, structure, `modDesc.xml`, mod IDs, versions and SHA-256 against the owner-reported export hashes.
- [ ] Inspect the actual `modDesc.xml` declarations requiring `FS25_AutoDrive` for A.P.S. and N.E.C.K.; test game auto-selection and missing dependency; test L.E.G.S. without AutoDrive.
- [ ] Review the separate BeatSync tool, rights, instructions and appropriate distribution. Do not treat it as a fourth mod ZIP.
- [ ] Keep A.S.S. within A.P.S.; exclude duplicate versions, DevTools and private packs.
- [ ] Test each module alone, A.P.S.+L.E.G.S., and the full combination; document dependencies accurately.
- [x] Record user-reported passing Lua tests: partial installations, missing/incompatible tour data, and module-text replacement with the same host (not independently verified in this documentation task).
- [ ] Verify the modular tour in game: registration, actual menu location, greyed-out missing modules, Deep Dive skipping, removed mods, differing UI/host revisions and DE/EN fallback.
- [ ] Verify the latest L.E.G.S. effects, world markers, force field and local map colours in game.
- [ ] Track H.E.A.D. visual testing separately in development; it is not a candidate for the three-mod package.
- [ ] Verify fresh installation, upgrades and any SmartGate/AutoDrive target migration.
- [ ] Record actually verified SP/MP/Dedi scenarios and clearly state unverified scenarios.
- [ ] Audit redistribution rights for the exact shipped code, media and assets.
- [ ] Receive and visually inspect all four planned GitHub PNGs, check provenance/rights and hashes, then add links to README and docs.
- [ ] Align README, changelog, known limitations, release notes and checksums with the **same** release payload.
- [ ] Obtain explicit owner approval before publishing a tag, release or ModHub submission.

### Documentation and update policy

The existing illustration catalogue is historical/supplemental, not proof of the current UI. Embedded tutorials can become the primary usage guide **after** their module-combination behavior is verified. Each central release records the actual version of each module; changing one module does not require a fake version increment for unchanged modules. No development candidate should be silently substituted for a released archive.
