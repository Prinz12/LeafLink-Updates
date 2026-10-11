# LeafLink Safe Firmware 3.2.3 Beta – Direktfunk nach Stromausfall

Lüfter halten ihre Verbindung zur Wall Control nach einem Neustart ohne
WLAN-Router aufrecht. Ihre regelmäßigen Funkmeldungen werden nun unabhängig
von einer LAN-Adresse bestätigt und bei Paketverlust wiederholt.

- Die gespeicherte Wall-Zuordnung bleibt auch bei länger ausgeschalteter
  Zentrale erhalten. Der Lüfter versucht die Funkverbindung erneut.
- Dies gilt auch für Geräte mit zusätzlich gespeicherten WLAN-Zugangsdaten.
- Bestätigungen für gleichzeitig neu gestartete Lüfter werden trotz gleicher
  Nachrichtenzähler getrennt verarbeitet.
- Die vorhandene Wall-Control-Firmware kann unverändert bleiben. Das Update
  ist nur auf den Lüftern erforderlich; Einstellungen und Funkformat bleiben erhalten.

## Zielgeräte und Installation

Profil: **Safe – Hardwareausgänge deaktiviert.** Für bestehende Safe-Geräte mit
ESP8266 ESP-12F, 4 MiB Flash und A/B-Bootlayout 2. Die Datei ist eine signierte
Update-Anwendung, kein vollständiges Flash-Abbild für Erstinstallation oder
Originalfirmware. Nicht mit einem generischen Upload ab Adresse 0 schreiben.

In der App unter Firmware-Updates „Beta-Versionen anzeigen“ einschalten.
Lüfter-OTA verwendet weiterhin den vorhandenen WLAN-Updateweg; ein Update über
die reine Direktfunkstrecke ist nicht enthalten. Nur an Wall Control gekoppelte
Geräte benötigen dafür eine WLAN-Einrichtung oder den kabelgebundenen Serviceweg.

## Prüfung

205 Firmware-Hosttests, 36 native Testprogramme, Codec-Interoperabilität,
Hardware-/Safe-Builds sowie Android-Hosttests, Build, Lint und Emulatorprüfungen
bestanden. Die native Funkprüfung deckt Paketverlust, über vier Stunden
simulierten Betrieb ohne LAN-Adresse, gleichzeitige Neustarts und die Rückkehr
der Zentrale ab. Ein Stromausfalltest dieser Version an echten Lüftern steht aus.

`version.json` enthält Profil, Layout, Größe, SHA-256 und Downloadlink.
Die Update-Datei verwendet den bestehenden LeafLink-Signaturschlüssel.
