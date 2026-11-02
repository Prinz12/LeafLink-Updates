# LeafLink 3.2.7 Beta – WLAN-Daten ohne Betriebsartwechsel

Die Übertragung gespeicherter WLAN-Daten durch Wall Control behält jetzt
die vorhandene Betriebsart des Lüfters bei. Ein direkt gekoppelter Lüfter
bleibt auch nach dem anschließenden Neustart im privaten Wall-Funknetz.
Ein bereits im WLAN betriebener Lüfter bleibt im WLAN-Betrieb.

Die neuen Zugangsdaten werden wie bisher zunächst durch eine echte Verbindung
geprüft und erst danach gespeichert. Funkbindung, Gruppe, Kanal und die
authentifizierte Betriebsartenkonfiguration werden dabei nicht überschrieben.
Bei einem Speicherfehler bleiben die bisherigen Zugangsdaten erhalten.
Ein Wechsel der Betriebsart ist weiterhin über einen ausdrücklichen
Rollenwechsel möglich. Die WLAN-Prüfung unterbricht den Direktfunk vorübergehend.

Enthält die USB-Startbestätigung und Stackkorrektur aus 3.2.6. Bootloader,
A/B-Layout, Signaturprüfung, Rückfall und spätere OTA-Updates bleiben erhalten.
Kompatibel mit Wall Control 0.5.7+, einschließlich der gespeicherten
WLAN-Weitergabe in 0.5.8/0.5.9. Kein Wall-/Display-Update erforderlich.

ESP8266 ESP-12F, 4 MiB, bestehendes A/B-Layout 2. Signiertes Anwendungsupdate,
kein Vollflash. Hardware aktiviert Ausgänge; Safe lässt sie deaktiviert.

Profil: **safe**.
