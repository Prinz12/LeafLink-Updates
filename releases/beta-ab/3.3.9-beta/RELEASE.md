# LeafLink 3.3.9 Beta – Mehr RAM für OTA-Updates

Die Firmware gibt vor einem Update zusätzliche Netzwerk-, Mesh- und Fleet-Puffer
frei und verkleinert den HTTP-Uploadpuffer. Am Testgerät standen dadurch während
der OTA-Vorbereitung rund 10 KiB mehr freier RAM zur Verfügung:
27.248 statt 16.744 Byte. Das verbessert die Reserve für Upload und Signaturprüfung.

Häufige Debug-Ausgaben sind im Normalbetrieb reduziert. Serielle Diagnose,
Herstellertest und Flasher-Protokolle bleiben verfügbar. Signaturprüfung,
Motorschutz, Speichergrenzen und A/B-Rückfall bleiben aktiv.

Vorhandene Kopplungen, WLAN-Daten, Hausplan, Nutzungszähler und Einstellungen
bleiben bei normalen Firmwareupdates erhalten. Ein Werksreset ist nicht nötig.
Ein zusätzliches App- oder Wall-Control-Update ist für diese Verbesserung nicht
erforderlich.

Geprüft wurden wiederholte signierte OTA-Updates, Uploadabbruch, ungültige
Signatur, gemischte Netzwerklast und serielle Diagnose am Testlüfter. Zusätzlich
bestanden 200 Firmware-Hosttests, 48 native Regressionstests, Protokoll- und
Sicherheitsprüfungen sowie Firmware- und Android-Builds, Lint und Emulatortests.
Die Prüfung umfasst einen realen Lüfter und kurze Lastläufe, keinen mehrtägigen
Dauertest.

Voraussetzung: ESP8266 ESP-12F mit 4 MiB Flash, Hardwareprofil und A/B-Layout 2.
In der App unter **Firmware-Updates** die **Beta-Versionen einschließen**, dann
**VERSION PRÜFEN** und **FIRMWARE HERUNTERLADEN** wählen. Anschließend die
gewünschten Lüfter über den bestehenden Updateablauf aktualisieren.
