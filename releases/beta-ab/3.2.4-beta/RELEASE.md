# LeafLink Firmware 3.2.4 Beta – OTA-Speicherreparatur

Behebt die wiederholte Meldung „Speicher knapp“ bei der OTA-Vorbereitung.
Der Berichtspuffer für den seriellen Fertigungstest wird erst bei einem
ausdrücklichen Testauftrag reserviert. Formattexte liegen im Flash.
Dadurch bleiben im normalen Betrieb rund 1,5 KiB zusätzlicher RAM frei.
OTA-Sicherheitsgrenzen und Signaturprüfung bleiben unverändert.

Die Direktfunk-Korrekturen aus 3.2.3 sind enthalten. Gespeicherte Einstellungen,
WLAN, Gruppen, Kopplungen und der Hausplan bleiben beim Firmware-Update erhalten.

## Zielgeräte und Installation

Profil: **Hardware – aktive Ausgänge.** Für ESP8266 ESP-12F mit 4 MiB Flash und
bestehendem LeafLink-A/B-Bootlayout 2. Signierte Update-Anwendung, kein vollständiges
Flash-Abbild. Nicht mit einem generischen Upload ab Adresse 0 installieren.

In der App: Firmware-Updates → Beta-Versionen anzeigen → Version prüfen.
OTA benötigt WLAN; die reine Direktfunkstrecke zur Wall Control überträgt keine
Firmware. Falls die installierte ältere Firmware schon die OTA-Vorbereitung
dauerhaft wegen Speichermangels ablehnt, ist zunächst eine datenbehaltende
USB-Reparatur nötig. Die neue Datei allein kann eine solche Sperre nicht beheben.

## Prüfung

Hardware und Safe gebaut und signiert; Firmware-Hosttests und native Tests
bestanden. Auf zwei Hardware-Testplatinen zunächst datenbehaltend installiert,
danach jeweils ein vollständiges signiertes WLAN-OTA mit bestätigtem Neustart
erfolgreich durchgeführt. Die Safe-Variante wurde nicht auf diesen Hardware-
Platinen installiert. Android-App und Updatekanal werden separat geprüft.

`version.json` enthält Profil, Layout, Größe, SHA-256 und Downloadlink.
Der bisherige LeafLink-Signaturschlüssel bleibt gültig.
