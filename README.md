# LeafLink Updates

Öffentlicher Updatekanal für die LeafLink-Android-App und die LeafLink-Firmware.

APK, Firmware als BIN und die zugehörigen Beschreibungen stehen unter [Releases](https://github.com/Prinz12/LeafLink-Updates/releases).
Die App prüft diesen Kanal ohne Anmeldung oder GitHub-Token. Die Installation erhält
die vorhandenen App-Daten. Geräte lassen sich nur innerhalb desselben Protokolls koppeln.

Kanal: `android-dual` · Release-Tags: `app-dual-v…` · Android-Paket: `de.prinz.leaflink`.
Die App prüft Dateigröße, SHA-256, Paketkennung, Versionscode und Signatur vor der Installation.

## Android-App 3.3.3

[App 3.3.3 herunterladen](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.3).
Bereits gekoppelte Handys öffnen die Gerätewebseite über **Einstellungen →
verbundene Geräte → WEB** ohne erneute Codeeingabe. Dafür ist Firmware 3.3.4
Beta erforderlich. Die App übergibt eine kurzlebige Freigabe; Gerätecode und
Kopplungsschlüssel bleiben geschützt. Kopplungen, Hausplan und Einstellungen
bleiben erhalten. Das App-Update allein installiert keine Lüfterfirmware.

### Sicherheitsumstellung ab App 3.3.0

[App 3.3.0 herunterladen und Updatebeschreibung lesen](https://github.com/Prinz12/LeafLink-Updates/releases/tag/app-dual-v3.3.0).
Die Version ergänzt Gerätecode-/QR-Kopplung, verschlüsselte LeafLink-Steuerung,
Handyzugänge und die Übernahme eines Wall-Funknetzes. Die vorhandene App erkennt
sie über **App-Update**. Android-Paket und Release-Signatur bleiben gleich.

Die LeafLink-Steuerung benötigt Firmware 3.3.0 und eine einmalige Kopplung mit
dem Gerätecode. Bei älterer LeafLink-Firmware zuerst die Sicherheitsumstellung
vorbereiten; das App-Update allein aktualisiert keine Lüfter. HAPLA wird weiterhin
separat unterstützt. Hinweise zur Wall-Migration stehen in der Updatebeschreibung.

App 3.2.2 korrigiert einen Fehlalarm nach erfolgreichen Firmware-Updates auf 3.2.0.
Bei einer bereits bestätigten Installation schließt **Firmware-Updates → Geräte
prüfen** den gespeicherten Vorgang durch Auslesen ab, ohne die Firmware erneut
zu übertragen. Änderungen an vorhandenen Einstellungen werden weiterhin erkannt.

## Firmware 3.3.4 Beta

[Signierte Hardware-Firmware 3.3.4 Beta herunterladen](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.4-beta).
Die Suche nach der zugeordneten Wall trennt ein funktionierendes WLAN nicht mehr.
Die vorhandene Wall-Zuordnung und gespeicherte Daten bleiben erhalten. Die
Weboberfläche unterstützt die automatische Freigabe durch App 3.3.3 sowie
alternativ den Gerätecode und eine optional gespeicherte Browsersitzung.

Die OTA-Speicherkorrekturen aus 3.3.3 bleiben enthalten. Eine sparsamere
Web-Routenverwaltung erhält den nötigen Arbeitsspeicher. Bei älteren Versionen,
die schon vor dem Upload an Speichermangel scheitern, ist einmalig eine
datenerhaltende USB-Serviceinstallation erforderlich.

In der App **Firmware-Updates → Beta-Versionen anzeigen → nach Updates suchen**.
Voraussetzung: Hardwareprofil, ESP8266 ESP-12F mit 4 MiB Flash und bestehendes
A/B-Layout 2. Die App prüft Profil, Layout, Größe, Hash und Signatur.
Für 3.3.4 wird kein Safe-Profil mehr angeboten; historische Releases bleiben erhalten.

Beim Wechsel von 3.2.x zuerst App 3.3.1 installieren und den individuellen
Gerätecode für die anschließende physisch freigegebene Kopplung bereithalten.
Bestehende Wall-Anlagen benötigen eine abgestimmte Sicherheitsumstellung;
die Voraussetzungen und der begrenzte Hardwareprüfstand stehen in der
[Updatebeschreibung](https://github.com/Prinz12/LeafLink-Updates/releases/tag/ab-v3.3.4-beta).
Das App-Update allein installiert keine Lüfterfirmware.

Dieses Repository enthält ausschließlich Release-Beschreibungen und
Updateinformationen; APKs und signierte BIN-Dateien liegen als Release-Downloads
bereit. Quellcode, Schlüssel und Gerätesicherungen werden nicht veröffentlicht.

## Wandbediengerät 0.5.1 Beta

[Update und Anleitung](https://github.com/Prinz12/LeafLink-Updates/releases/tag/wall-v0.5.1-beta)
für LILYGO T-Display (16 MiB) und Nextion NX4827K043_011.
Kanal `wall-beta`, Tag-Präfix `wall-v`, Manifest `manifest.json`.
Installation über die authentifizierte Weboberfläche; die Android-App filtert
diesen separaten Kanal aus. HMI 302 bleibt unverändert.

Wall Control 0.5.1 korrigiert den schnellen Rückwechsel ins Heim-WLAN unmittelbar nach einer Neugerätesuche. 0.5.0 wird dadurch ersetzt; bitte 0.5.1 verwenden.
