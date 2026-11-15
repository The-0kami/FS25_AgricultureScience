# Installation – Agriculture Science (LS25)

> **Aktueller Stand: 15.11.2026 · Release in Vorbereitung.** Es gibt noch keine veröffentlichten GitHub-Release-Assets. Diese Anleitung beschreibt die drei geprüften lokalen Release-Kandidaten; die endgültige Freigabe und MP-/Dedi-Prüfungen sind noch offen.

## Pakete

| Datei | Modul | Version |
|---|---|---|
| `FS25_APS_AgricultureScience.zip` | **A.P.S.**, einschließlich A.S.S. | 1.0.0.0 |
| `FS25_SmartGate_AgricultureScience.zip` | **L.E.G.S.** | 1.0.0.0 |
| `FS25_NECK_AgricultureScience.zip` | **N.E.C.K.** | 0.1.0.0 |

**AutoDrive separat installieren:** A.P.S. und N.E.C.K. deklarieren `FS25_AutoDrive` in der jeweiligen `modDesc.xml` als notwendige Abhängigkeit. Die verwendete Referenz ist AutoDrive **3.0.1.4**, nicht eine bestätigte Mindestversion. L.E.G.S. kann eigenständig genutzt werden. A.S.S.-Servicefunktionen setzen A.P.S. **und** L.E.G.S. voraus. Courseplay ist optional.

## Neuinstallation

1. LS25 vollständig beenden; Spielstand und Mods sichern.
2. Nach Freigabe die gewünschten **einzelnen Mod-ZIPs** von [GitHub Releases](https://github.com/The-0kami/FS25_AgricultureScience/releases) herunterladen. Das automatisch erzeugte GitHub-Quellcode-ZIP ist **keine Spielmod**.
3. Ein optionales äußeres *Complete*-ZIP zuerst entpacken. Die **inneren Mod-ZIPs nicht entpacken**.
4. Die einzelnen ZIPs unverändert in den aktiven LS25-Modordner kopieren. Alte oder doppelte Installationen entfernen.
5. AutoDrive separat bereitstellen, benötigte Mods im Spielstand aktivieren, Menü und Funktionen prüfen.

## Updates und Server

Vor Updates zusätzlich die bisherige `smartGate.xml` und AutoDrive-Ziele sichern. Für ältere LEGS-Service-Bays mit numerischen AD-Zielen kann eine erneute Auswahl des Ziels nötig sein: [Migrationshinweise](MIGRATION_AD_TARGETS.md). Für MP/Dedi müssen Clients und Server **bytegleiche Mod-ZIPs** einsetzen; Prüfsummen statt nur Versionsnummern vergleichen. Der vollständige aktuelle End-to-End-Test auf Dedicated Servern ist noch nicht abgeschlossen.

## Einrichten und Hilfe

[A.P.S.-Tutorial](TUTORIAL_APS.md) · [A.S.S.-Tutorial](TUTORIAL_ASS.md) · [L.E.G.S.-Tutorial](TUTORIAL_LEGS.md) · [Fehlerdiagnose](TROUBLESHOOTING.md) · [Kompatibilität](../COMPATIBILITY.md)

**Hinweis zu älteren Illustrationen:** Die am 29.10.2026 erzeugten UI-Bilder sind codebasierte Vorschauen und keine Ingame-Screenshots. Die neuen DE/EN-GUI-Vorschauen vom 15.11.2026 werden separat für die GitHub-Dokumentation vorbereitet.
