# Fehlerdiagnose und Bugreports

Vor einem Test **Mod-ZIPs anhand SHA-256 identifizieren**, nicht nur `1.0.0.0` ablesen. [Build-Matrix](../BUILD_STATUS.md). LS25- und AD-Version, SP/Host/Dedi, Fahrzeug und Anbaugeräte, Auftrag und aktuelle bereinigte Logs dokumentieren.

| Symptom | Was zuerst prüfen? |
|---|---|
| **Fahrt zum falschen Serviceort** | Tatsächlichen SG-Build, aktuelle AD-Liste und gespeichertes Bay-Ziel prüfen. Im **noch nicht installierten 29.10.-Kandidaten** alte positive Ziele **einmal neu wählen**, um Name/Position zu erfassen. [Migration](MIGRATION_AD_TARGETS.md). |
| **Kein passender Provider/keine Quelle** | Native unterstützte Quelle, Providerrahmen, Farmrechte, `OPEN`, Energieart und echte Gebäudetrigger. Deko-Tanks sind keine Tankquelle; öffentliche Quellen benötigen native Freigabe. |
| **Bay UNKNOWN** | UNKNOWN ist konservativ und **nicht FREE**. Geometrie, lokale Objekte/Paletten, gekippte Bodies und aktuelle Belegung prüfen. Entfernte Objekte außerhalb der Bay nicht pauschal verantwortlich machen; echte lokale Blocker nicht ignorieren. |
| **Bay belegt/reserviert** | Physisches `OCCUPIED` und separate `RESERVED`-Lease prüfen. Anfrage später erneut auslösen: **keine aktive Service-Warteschlange**. |
| **Service startet, Effekt fehlt** | Native Wirkzone gegen sämtliche nötigen Gespannteile prüfen. Animation allein bedeutet keine Reinigung/Reparatur/Betankung. Bei Bühnen Absenken vor Abfahrt kontrollieren. |
| **AD-Ziel existiert, Anfahrt scheitert** | AD-Konnektivität und tatsächlich befahrbaren Weg prüfen. Zielmarker ist kein Routennachweis. |
| **Parken nach Hinweis nicht fortgesetzt** | **Aktuellen Serverlog** samt Auftrag/Job-ID und AD-Pfadfehlern erfassen; der historisch offene Fall gilt nicht generell als behoben. |
| **Kein Beleg/keine Stimme** | Lokale Audio-/Druckeroptionen, sichere Spieler-/Sitzungszuordnung, vorhandene Clips prüfen. Nicht zugeordnete automatische Aufträge erzeugen nicht automatisch private Darstellung. |
| **Alte Voice-Line nach Update** | Externe Packs unter `modSettings/APS_sounds/voices/` werden nicht pauschal überschrieben. Vor manuellem Austausch persönliche Änderungen sichern. |
| **Controller findet Serviceeditor nicht vollständig** | Zentraler Agriculture-Science-Reiter hat Controllerpfade; der separate **Inworld-Serviceeditor** ist noch nicht vollständig controllerbedienbar. |

## Umfang eines guten Fehlerberichts

- LS25-Version und AutoDrive-Version; genaue **APS-/SG-SHA-256**.
- Singleplayer, Hosted Multiplayer oder Dedicated Server; bei MP: welcher Client/Host.
- Fahrzeugmodell, Anbaugeräte, Füll-/Schadenszustände.
- Provider-/Bay-Konfiguration, Fähigkeiten, Quellen, AD-Ziel und Belegungsstatus.
- Reproduzierbare Schritte sowie tatsächliches/erwartetes Verhalten.
- **Aktueller**, auf private Daten bereinigter `log.txt`-Ausschnitt mit relevanten Auftrag-/Job-IDs.
- Bei neuer AD-Zielbindung: wurde das Ziel nach Installation bewusst neu ausgewählt?

Automatisierte Regressionen sind kein Ingame-/Dedi-Beweis. Keine Erklärung als bestätigt bezeichnen, die lediglich eine plausible Vermutung ist.
