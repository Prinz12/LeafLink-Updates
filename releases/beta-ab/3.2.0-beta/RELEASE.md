# LeafLink Firmware 3.2.0 Beta – Räume und Lüftungsgruppen

Signierte A/B-Firmware für den normalen Lüfterbetrieb. Die BIN-Datei steht ohne
Anmeldung zum Download bereit.

## Änderungen

- Der physische Aufstellraum wird unabhängig von der Lüftungsgruppe im Gerät gespeichert.
- Zwei Lüfter können im selben Raum oder in verschiedenen Räumen eine Gruppe bilden.
- Bestehende Paarungen bleiben beim Upgrade erhalten. Die Raumzuordnung ist mit LeafLink App 3.2.0 bedienbar.
- Raumänderungen prüfen die Gerätekennung und die bisherige Gruppe. Die Speicherung wird bestätigt und kann getrennt zurückgelesen werden.
- Die Feuchteregelung berücksichtigt den höchsten gültigen Messwert der Gruppe. Zeitgrenzen, Nachtmodus und Schutz bei veralteten Messwerten bleiben erhalten.

## Passende Geräte

Nur für bereits eingerichtete LeafLink-Geräte mit ESP8266 ESP-12F, 4 MiB Flash,
A/B-Layout 2 und Hardware-Profil. Originalfirmware und HAPLA sind nicht kompatibel.
`firmware.bin` ist ein signiertes Firmware-Update, kein vollständiges Flash-Abbild
und kein Ersatz für den A/B-Bootloader. Die Datei nicht als komplettes Abbild ab
Flash-Adresse 0 schreiben. Für das Safe-Profil gibt es eine separate Veröffentlichung.

Ältere Konfigurationen werden übernommen. Firmware 3.0.0 kann das neue
Konfigurationsformat nicht lesen; für einen späteren Rückgang ist die passende
vollständige Gerätesicherung erforderlich.

## Dateien und Prüfung

- `firmware.bin`: signiertes Update für das Hardware-Profil.
- `version.json`: Version, Geräteprofil, Layout und öffentlicher Downloadlink.
- `SHA256SUMS`: Prüfsumme der BIN-Datei.
- `RELEASE.md`: diese Beschreibung.

196 Firmwaretests, 30 native Testprogramme, Protokolltests und alle vier
Firmware-Builds bestanden. Diese Hardware-Version wurde zusätzlich auf einem
Testgerät geprüft, einschließlich Raumzuordnung, Neustart und erhaltener Paarung.
Signatur und SHA-256 wurden vor der Veröffentlichung erneut geprüft.
