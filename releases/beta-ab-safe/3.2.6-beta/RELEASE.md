# LeafLink 3.2.6 Beta – bestätigter USB-Start ohne WLAN

Korrigiert die USB-Installation bei Lüftern, die ausschließlich im privaten
Wall-Control-Funknetz laufen. Bisher setzte die dauerhafte A/B-Übernahme einen
HTTP-Statusabruf voraus; ohne WLAN fiel das Gerät auf die vorige Version zurück.

Neu ist eine Statusabfrage mit Empfangsbestätigung über den seriellen Anschluss.
Der Installationsleser prüft Gerätekennung, Profil, Version, Image-Hash und CRC
und quittiert genau die empfangene Antwort innerhalb von fünf Sekunden.
Eine bloße USB-Verbindung oder ein Neustart bestätigt das Update nicht.
Die zehn Sekunden gesunder Hauptlauf, Initialisierung, Motorfehlerprüfung und
der dauerhafte A/B-Commit bleiben erforderlich. HTTP-Updates funktionieren
weiterhin über ihren bisherigen Bestätigungsweg. Ein USB-Installationswerkzeug
muss die neue Statusabfrage unterstützen; bloßes Schreiben des BIN reicht bei
Lüftern ohne HTTP-Zugang weiterhin nicht aus.

Behebt außerdem einen Stacküberlauf bei Sensorabfragen im privaten Funknetz:
Die temporären Daten der WLAN-Weitergabe werden nicht mehr in die Hauptschleife
eingebettet. Ein Buildtest begrenzt deren Stackrahmen auf 448 Byte statt 976.
Der Bootloader, das A/B-Layout, Signaturprüfung und OTA-Uploadweg bleiben erhalten.

Enthält die verschlüsselte WLAN-Weitergabe aus 3.2.5 mit Wall Control 0.5.7:
Option „WLAN-Daten auch an Lüfter übertragen“, zunächst ausgeschaltet.
WLAN-Daten, Gruppen und private Funkbindung bleiben beim Update erhalten.
Ein realer WLAN-Wechsel wurde bei dieser Veröffentlichung nicht durchgeführt.

ESP8266 ESP-12F, 4 MiB, bestehendes A/B-Layout 2. Signiertes Anwendungsupdate,
kein Vollflash. Hardware aktiviert Ausgänge; Safe lässt sie deaktiviert.

Profil: **safe**.
