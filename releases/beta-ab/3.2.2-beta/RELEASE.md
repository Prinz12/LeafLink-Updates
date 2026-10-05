# LeafLink Firmware 3.2.2 Beta – Hardware

Direktfunk-Erstaufnahme fabrikneuer Lüfter über Wall Control 0.5.0: Taster kurz
drücken, innerhalb des dreiminütigen Kopplungsfensters Gerät und individuellen
Einrichtungscode auswählen, Gruppe festlegen und Aufnahme bestätigen. Der Code
wird für das Geräteetikett ausdrücklich über USB/UART abgerufen. Bereits
eingerichtete Geräte werden nicht neu provisioniert; vorhandene Einstellungen
bleiben erhalten.

X25519, authentifizierter Sitzungsaustausch und AES-256-GCM schützen die
Übertragung. Eigenständige Funkzugangsdaten werden im Lüfter verschlüsselt und
authentifiziert gespeichert. Der Abschluss benötigt eine tatsächliche
Rückmeldung im Direktfunknetz; unterbrochene Vorgänge bleiben überprüfbar.

**Beta-Grenze:** Die vollständige Erstaufnahme eines fabrikneuen realen Geräts
ist noch nicht Ende zu Ende geprüft. Die fünf eingerichteten Testgeräte werden
dafür nicht zurückgesetzt. Unveränderte Originalhersteller-Firmware unterstützt
diesen Kopplungsweg nicht. Lüfter-OTA über reinen Direktfunk ist nicht enthalten;
Updates benötigen WLAN oder den dokumentierten kabelgebundenen Serviceweg.

RSA-signierte A/B-Anwendung für ESP8266 ESP-12F mit 4 MiB und vorhandenem
Bootlayout 2; keine vollständige Erstinstallation und kein generischer
PlatformIO-Upload. Dieses Hardware-Profil kann die Hardwareausgänge ansteuern.

Geprüft: 495 Kryptografieprüfungen, 205 Hosttests und 35 native Testprogramme; Hardware- und Safe-Builds einschließlich A/B. Der Kryptografie-Selbsttest wurde auf ESP8266 und ESP32 erfolgreich ausgeführt. Die noch offene Erstaufnahme-Abnahme bleibt oben ausdrücklich beschrieben.
