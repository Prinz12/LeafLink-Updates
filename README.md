# LeafLink Updates

Öffentlicher Updatekanal für die LeafLink-Android-App und die LeafLink-Firmware.

APK, Firmware als BIN und die zugehörigen Beschreibungen stehen unter [Releases](https://github.com/Prinz12/LeafLink-Updates/releases).
Die App prüft diesen Kanal ohne Anmeldung oder GitHub-Token. Die Installation erhält
die vorhandenen App-Daten. Geräte lassen sich nur innerhalb desselben Protokolls koppeln.

Kanal: `android-dual` · Release-Tags: `app-dual-v…` · Android-Paket: `de.prinz.leaflink`.
Die App prüft Dateigröße, SHA-256, Paketkennung, Versionscode und Signatur vor der Installation.

App 3.2.2 korrigiert einen Fehlalarm nach erfolgreichen Firmware-Updates auf 3.2.0.
Bei einer bereits bestätigten Installation schließt **Firmware-Updates → Geräte
prüfen** den gespeicherten Vorgang durch Auslesen ab, ohne die Firmware erneut
zu übertragen. Änderungen an vorhandenen Einstellungen werden weiterhin erkannt.

## Firmware 3.2.2 Beta

3.2.2 ergänzt die Direktfunk-Erstaufnahme über Wall Control 0.5.1 mit
physisch geöffnetem Kopplungsfenster, individuellem Einrichtungscode und
Gruppenwahl. Bestehende Einstellungen bleiben erhalten. Ein vollständiger
Erstkopplungstest mit fabrikneuer Hardware steht noch aus; diese Funktion
ist als Beta zur Erprobung veröffentlicht. Die vorherige Direktfunksteuerung
bereits eingerichteter Geräte bleibt enthalten.

Die Firmware speichert den Aufstellraum getrennt von der Lüftungsgruppe. Ein Paar
kann im selben Raum oder in verschiedenen Räumen arbeiten. Bestehende Kopplungen
bleiben erhalten. Die Feuchteregelung berücksichtigt den höchsten gültigen
Messwert der Gruppe.

| Variante | Download und Beschreibung | Verwendung |
| --- | --- | --- |
| Normal | [A/B-Firmware 3.2.2 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.2.2-beta) | Betrieb mit aktiven Hardware-Ausgängen |
| Safe | [A/B-Safe-Firmware 3.2.2 Beta](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-safe-v3.2.2-beta) | Testbetrieb mit deaktivierten Hardware-Ausgängen |

Beide Varianten sind signierte Updates für bereits eingerichtete LeafLink-Geräte
mit ESP8266 ESP-12F, 4 MiB Flash und A/B-Layout 2. Sie sind keine vollständigen
Flash-Abbilder und nicht für Geräte mit Originalfirmware bestimmt. Das passende
Profil muss beibehalten werden. Versionsinformationen und SHA-256-Prüfsummen
liegen jeder Veröffentlichung bei. Der Download ist ohne Anmeldung möglich.

Ab App 3.2.1 erfolgen auch Firmware-Suche und BIN-Downloads über diesen öffentlichen
Kanal ohne GitHub-Anmeldung. Unter Firmware-Updates „Beta-Versionen anzeigen“
aktivieren, um die aktuelle Firmware 3.2.2 Beta zu sehen. Die App prüft Dateigröße,
Prüfsumme, Signatur, Geräteprofil und A/B-Layout. Ältere App-Versionen zunächst
über App-Update aktualisieren.

Dieses Repository enthält ausschließlich Release-Beschreibungen und
Updateinformationen; APKs und BIN-Dateien liegen als Release-Downloads bereit.
Der Entwicklungsquellcode wird privat verwaltet. Die Firmware wird durch ein
App-Update nicht verändert.

## Wandbediengerät 0.5.1 Beta

[Update und Anleitung](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.5.1-beta)
für LILYGO T-Display (16 MiB) und Nextion NX4827K043_011.
Kanal `wall-beta`, Tag-Präfix `wall-v`, Manifest `manifest.json`.
Installation über die authentifizierte Weboberfläche; die Android-App filtert
diesen separaten Kanal aus. HMI 302 bleibt unverändert.

Wall Control 0.5.1 korrigiert den schnellen Rückwechsel ins Heim-WLAN unmittelbar nach einer Neugerätesuche. 0.5.0 wird dadurch ersetzt; bitte 0.5.1 verwenden.
