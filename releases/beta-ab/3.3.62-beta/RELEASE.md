# LeafLink 3.3.62 Beta – Sommermessung und Tastenbedienung

Nach einer Änderung der Sommer-Einstellungen wird der Motorbefehl für die neue
Messung zuverlässig erneut gesetzt. Ein gespeicherter alter Befehl konnte den
sofortigen Wiederanlauf bisher verhindern.

Kurze Tastendrücke werden jetzt anhand einer festen Entprellzeit erkannt.
Netzwerk- und Sensorarbeit verlängert diese Zeit nicht mehr durch das Zählen
von Hauptschleifendurchläufen. Schutz und Bestätigung bei langen Tastendrücken
bleiben erhalten.

Die Taste schaltet weiterhin die Gruppen-Leistungsstufe. Während einer
Sommermessung begrenzt die konfigurierte Messleistung auch höhere Stufen;
in einer regulären Automatikpause bleibt der Motor stehen. Beim Beginn einer
neuen Messung erscheinen Temperaturwerte erst wieder nach Stabilisierung.

Beide Fehler wurden mit dem tatsächlichen Firmwarecode in Regressionstests
nachgewiesen und korrigiert. Der Ablauf mit Einstellungswechsel, Messung und
Tastenbedienung wurde zusätzlich an zwei Geräten mit der bisherigen Firmware
untersucht. Ein dauerhafter vollständiger Stillstand ließ sich dabei nicht
reproduzieren. Diese neue Firmware wurde noch nicht auf einem Gerät installiert.

Kopplungen, WLAN-Daten, Hausplan und Einstellungen bleiben beim normalen Update
erhalten. Kein zusätzliches App- oder Wall-Control-Update erforderlich.

In der App unter **Firmware-Updates** die **Beta-Versionen anzeigen**, dann
**VERSION PRÜFEN** und **FIRMWARE HERUNTERLADEN** wählen. Installation durch den
Nutzer. Voraussetzung: Hardwareprofil, ESP8266 ESP-12F mit 4 MiB und A/B-Layout 2.

Das zugehörige Lizenz-/LGPL-Paket ist bei dieser Veröffentlichung beigefügt;
es ist kein OTA-Update. Details stehen in LGPL.md.
