# LeafLink Android 3.2.1 – Öffentliche Firmware-Updates

Firmware-Versionen prüfen und BIN-Dateien herunterladen funktioniert jetzt über
den öffentlichen LeafLink-Updatekanal ohne GitHub-Anmeldung oder Token.

- Die bisherige Einrichtung eines privaten Update-Zugangs entfällt.
- Normale Firmware und Safe-Version werden getrennt erkannt und mit ihrer Beschreibung angezeigt.
- Dateigröße, Prüfsumme, Signatur, Geräteprofil und A/B-Layout werden weiterhin geprüft.
- Gespeicherte unterbrochene Updates bleiben nach dem Wechsel des Downloadkanals lesbar.
- Räume, Lüftungsgruppen und die Unterstützung von HAPLA- und LeafLink-Geräten bleiben erhalten. Gruppen können weiterhin nur Geräte desselben Protokolls enthalten.

Unter **Firmware-Updates → Beta-Versionen anzeigen** die Beta-Auswahl aktivieren,
um die veröffentlichte Firmware 3.2.0 Beta zu sehen. Ein App-Update installiert
keine Firmware automatisch auf den Lüftern.

Die APK wird als Update über die vorhandene LeafLink-App installiert. Paketkennung
und Signaturschlüssel bleiben gleich; vorhandene App-Daten bleiben erhalten.

Geprüft im virtuellen Android: reale öffentliche Versionsprüfung und Downloads
beider signierter Firmware-Dateien, 176 Firmware-Update-Prüfungen sowie 26
Raumgruppen-Prüfungen. Android-Build und Prüflauf ohne Fehler.
