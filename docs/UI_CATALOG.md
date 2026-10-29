# UI-Katalog / UI catalogue

## Deutsch

**48 ausgewählte Abbildungen: 24 Schritte/Zustände jeweils auf Deutsch und Englisch.** Grundlage ist der Katalog vom 29.10.2026 mit 127 Einzelbildern. Das ZIP enthält zusätzlich eine PNG-Vorschau und einen JPG-Kontaktbogen, insgesamt 129 Bilddateien. ZIP-CRC und vollständiges Decodieren aller Bilder wurden lokal geprüft.

**Keine Ingame-Screenshots:** Die Abbildungen stammen aus echten Lua-Zeichenaufrufen, aus den tatsächlichen Settings-Controls mit vereinfachter XML-Layoutrekonstruktion oder aus Quelltexten in angenäherten nativen Dialogflächen. Der Zonenplan ist eine schematische Draufsicht echter Debug-Line-Koordinaten. Segoe UI ersetzt die Engine-Schrift; Farben, Fensterrahmen, Umbruch, Fokus und HDR können abweichen. Beispielnamen, Fahrzeug, Mengen und Preise sind Testdaten und kein Servicenachweis. Die Settings-Bildseiten sind Dokumentationsausschnitte, keine neuen Unterseiten im Spiel.

Die Quellen enthalten den SmartGate-Kandidaten `SG_InteractionDescription_20261029` einschließlich AD-Zielidentität. Lokal installiert und geprüft bedeutet **keine** SP-/Dedi-Abnahme. Der native Benennungsdialog wurde zuvor vom Nutzer in SP und Dedi bestätigt; diese Rekonstruktion ersetzt die Prüfung nicht. [Buildstatus](BUILD_STATUS.md).

Die öffentlichen PNGs wurden verlustfrei neu komprimiert und von Metadaten befreit. Pixel, Auflösung und Seitenverhältnis sind unverändert. Keine Schwärzung war nötig; keine UI-Elemente ergänzt. Die Originale bleiben lokal erhalten. Die englischen Bilder verwenden englische UI-Texte, können jedoch deutsche frei vergebene Gebäude-/Bay-Namen enthalten. Der technische Namenshinweis `sgServiceName` ist eine bestehende Quellstand-Eigenheit und keine empfohlene Eingabe.

**Bewusst nicht ausgewählt:** Debugansichten, redundante Zustände, Übergangsframes, das neutrale Voice-Overlay außerhalb dieses Tutorialumfangs und eine künstliche Testkonfiguration mit allen Fähigkeiten an einer Waschquelle. Diese würde eine nicht bewiesene Mehrfach-Servicequelle suggerieren. Private Ordis-/Warframe-Assets sind nicht enthalten. Texte und eigene Projektgrafiken sind für diese Projektdokumentation freigegeben; daraus folgt keine pauschale CC0-Freigabe aller Assets. Es werden keine Schriftdateien oder fremden HUD-/Grafikdateien verteilt.

### Noch benötigte echte Aufnahmen

- AD-Fahrzeug-/Geräteparkziel-Zuweisung und APS-Parkbutton im AD-HUD.
- Vollständiger Lernablauf mit einem konkreten Gerät.
- Erkennung und Auswahl eines Tores sowie Weltansicht aller Zonen mit Fahrzeug im Safety-Bereich.
- Verknüpftes REPAIR-/Hebebühnenprofil und angehobene/abgesenkte Plattform.
- Verifiziertes REFUEL-/CHARGE-Stationsprofil mit passendem Energieverbraucher.
- Native Rückkehrfahrt, Beleganimation und Migration im aktuellen SP-/Dedi-Kandidaten.

Keine fehlende Aufnahme wurde durch eine erfundene Bedienoberfläche ersetzt. Nicht enthaltene Funktionen wie ausführende FIFO-Schlange, Massenwartung, fertiger globaler Statusmonitor und N.E.C.K. werden nicht bebildert.

## English

**48 selected illustrations: 24 matching steps/states in German and English.** The source catalogue contains 127 individual illustrations plus a PNG preview and a JPG contact sheet, for 129 image files inside the ZIP. CRC and full image decoding passed locally.

**Not in-game screenshots:** Methods are actual Lua draw-call replay, actual settings controls with simplified XML layout reconstruction, source text in approximated native dialog shells, and a schematic top view based on actual debug-line coordinates. Segoe UI substitutes for the engine font; color, window styling, wrapping, focus and HDR may differ. Demo names, vehicle, quantities and prices prove no actual service result. Paginated settings illustrations are documentation crops, not additional game pages.

Source state includes `SG_InteractionDescription_20261029` and the AD-target identity fix. Local installation and automated tests are **not** native SP/Dedi approval. Previous native rename-dialog behavior was user-confirmed on SP and Dedi; these reconstructions are not substitutes. See [build status](BUILD_STATUS.md).

Public PNGs use lossless recompression and no metadata. Pixels, dimensions and aspect ratio are unchanged. No redaction or added UI was needed; originals remain local. English UI examples may retain German user/building names. The source-derived `sgServiceName` technical hint is not a recommended key binding.

**Excluded:** Internal debug views, redundant states, animation intermediate frames, the neutral voice overlay outside this tutorial scope, and an artificial fixture assigning all capabilities to a wash source. No private Ordis/Warframe assets, external HUD graphics or font files are included. Project graphics/text are used with owner authorization for project documentation; no blanket CC0 license is inferred.

### Missing native captures

- AD vehicle/implement parking-target assignment and APS parking-button integration.
- A complete teaching workflow for an actual implement.
- Gate discovery/selection and world-space zones with a vehicle inside safety.
- A linked REPAIR/lift profile and raised/lowered platform.
- Verified REFUEL/CHARGE station setup with a matching energy consumer.
- Native return driving, receipt animation and migration on the current SP/Dedi candidate.

No missing capture is replaced with an invented interface. Executing FIFO queues, mass maintenance, a finished global status monitor and N.E.C.K. are not illustrated as implemented features.

## Inventory and provenance / Inventar und Herkunft

- [All 127 images and selection decisions](assets/ui/INVENTORY.csv)
- [Selected-image hashes, source hashes and rendering methods](assets/ui/MANIFEST.json)

Lossless PNG bytes, selected images: **5,743,370 → 5,603,127** (2.4% reduction). Original dimensions preserved.

## Galerie / Gallery

Each row links to full-resolution DE and EN images. / Jede Zeile verlinkt die unskalierten DE-/EN-Bilder.

| Step / Schritt | DE | EN |
|---|---|---|
| Agriculture Science overview with three available module cards. | [DE](assets/ui/common/as_modules_de.png) | [EN](assets/ui/common/as_modules_en.png) |
| Example of a disabled A.S.S. card when its view is not ready. | [DE](assets/ui/common/as_module_unavailable_de.png) | [EN](assets/ui/common/as_module_unavailable_en.png) |
| Global A.P.S. implement-parking and job-end takeover options. | [DE](assets/ui/aps/aps_parking_settings_de.png) | [EN](assets/ui/aps/aps_parking_settings_en.png) |
| Manual teaching required: actual message text in an approximated notification surface. | [DE](assets/ui/aps/aps_teach_required_de.png) | [EN](assets/ui/aps/aps_teach_required_en.png) |
| Gate profile with automatic pre-opening and opening, closing and safety dimensions. | [DE](assets/ui/legs/legs_gate_auto_de.png) | [EN](assets/ui/legs/legs_gate_auto_en.png) |
| Per-gate manual lookahead; the shown distance is a demo value. | [DE](assets/ui/legs/legs_gate_manual_de.png) | [EN](assets/ui/legs/legs_gate_manual_en.png) |
| Animation direction is inverted; approach detection is unchanged. | [DE](assets/ui/legs/legs_gate_inverted_de.png) | [EN](assets/ui/legs/legs_gate_inverted_en.png) |
| Interactable profile triggered on entry, without an empty Detected row. | [DE](assets/ui/legs/legs_interactive_tripwire_de.png) | [EN](assets/ui/legs/legs_interactive_tripwire_en.png) |
| Schematic top view: cyan opening, purple closing, red safety. Not a world-space game view. | [DE](assets/ui/legs/legs_trigger_zones_de.png) | [EN](assets/ui/legs/legs_trigger_zones_en.png) |
| Global discovery, pre-opening action and default activation of new gates. | [DE](assets/ui/legs/legs_discovery_preopen_settings_de.png) | [EN](assets/ui/legs/legs_discovery_preopen_settings_en.png) |
| Management: select, create and name areas and bays; candidate and template actions below. | [DE](assets/ui/ass/ass_service_management_de.png) | [EN](assets/ui/ass/ass_service_management_en.png) |
| Edit: provider bounds. This limits source selection and is not the bay occupancy area. | [DE](assets/ui/ass/ass_provider_bounds_de.png) | [EN](assets/ui/ass/ass_provider_bounds_en.png) |
| Edit: service bay. X/Z, width, height, length and orientation apply to the selected bay. | [DE](assets/ui/ass/ass_bay_geometry_de.png) | [EN](assets/ui/ass/ass_bay_geometry_en.png) |
| Selected bay AD target: manual selection, search, refresh and nearby-marker suggestion. | [DE](assets/ui/ass/ass_ad_destination_de.png) | [EN](assets/ui/ass/ass_ad_destination_en.png) |
| Wash example: native source linked, WASH enabled, operational OPEN and occupancy FREE. | [DE](assets/ui/ass/ass_wash_source_de.png) | [EN](assets/ui/ass/ass_wash_source_en.png) |
| Current help for capabilities, automatic stations, lift holding and energy types; dialog shell approximated. | [DE](assets/ui/ass/ass_service_help_de.png) | [EN](assets/ui/ass/ass_service_help_en.png) |
| UNKNOWN occupancy: not available, even when operational state is OPEN. | [DE](assets/ui/ass/ass_bay_unknown_de.png) | [EN](assets/ui/ass/ass_bay_unknown_en.png) |
| Example showing physical OCCUPIED plus a separate RESERVED reservation. | [DE](assets/ui/ass/ass_bay_occupied_reserved_de.png) | [EN](assets/ui/ass/ass_bay_occupied_reserved_en.png) |
| Three manual service requests and automatic wash options on the A.S.S. page. | [DE](assets/ui/ass/ass_manual_requests_wash_de.png) | [EN](assets/ui/ass/ass_manual_requests_wash_en.png) |
| Automation and thresholds: remaining vehicle condition and remaining fuel or charge. | [DE](assets/ui/ass/ass_condition_energy_thresholds_de.png) | [EN](assets/ui/ass/ass_condition_energy_thresholds_en.png) |
| Maximum service time, no-progress limit and optional local ticket printer. | [DE](assets/ui/ass/ass_monitoring_receipt_settings_de.png) | [EN](assets/ui/ass/ass_monitoring_receipt_settings_en.png) |
| Local completed REPAIR receipt. Workshop items are humorous text; demo data. | [DE](assets/ui/ass/ass_receipt_repair_de.png) | [EN](assets/ui/ass/ass_receipt_repair_en.png) |
| REFUEL example with observed quantity and estimated balance delta, not an isolated station invoice. | [DE](assets/ui/ass/ass_receipt_refuel_de.png) | [EN](assets/ui/ass/ass_receipt_refuel_en.png) |
| Rename an area; an empty name uses automatic numbering. Native dialog styling approximated. | [DE](assets/ui/ass/ass_rename_area_de.png) | [EN](assets/ui/ass/ass_rename_area_en.png) |
