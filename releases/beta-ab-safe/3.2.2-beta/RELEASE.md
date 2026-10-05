# LeafLink Firmware 3.2.2 Beta – Safe

Direktfunk-Erstaufnahme fabrikneuer Lüfter über Wall Control 0.5.0 mit
deaktivierten Hardwareausgängen. Taster kurz drücken, im dreiminütigen
Kopplungsfenster Gerätekennung und individuellen Einrichtungscode auswählen,
Gruppe festlegen und Aufnahme bestätigen. Für die Geräteetikettierung kann der
Code ausdrücklich über USB/UART abgerufen werden. Bereits eingerichtete Geräte
sind vor dieser Erstaufnahme geschützt; bestehende Einstellungen bleiben erhalten.

X25519, authentifizierter Sitzungsaustausch und AES-256-GCM sichern die Aufnahme;
die eigenständigen Funkzugangsdaten werden im Lüfter verschlüsselt und
authentifiziert gespeichert. Erfolg wird erst nach einer frischen Rückmeldung
im Direktfunknetz angezeigt. Unterbrochene Vorgänge bleiben überprüfbar.

**Beta-Grenze:** Eine vollständige Erstaufnahme auf fabrikneuer realer Hardware
ist noch nicht Ende zu Ende geprüft. Die vorhandenen fünf eingerichteten Geräte
werden dafür nicht zurückgesetzt. Originalhersteller-Firmware unterstützt
diesen Weg nicht. Lüfter-OTA über ausschließlich Direktfunk ist nicht enthalten;
Updates benötigen WLAN oder den dokumentierten kabelgebundenen Serviceweg.

RSA-signierte A/B-Anwendung für ESP8266 ESP-12F mit 4 MiB und vorhandenem
Bootlayout 2. Keine vollständige Erstinstallation und kein generischer
PlatformIO-Upload. Safe darf nicht als Nachweis funktionierender Motoransteuerung
oder gemessener Luftleistung verstanden werden.

Geprüft: 495 Kryptografieprüfungen, 205 Hosttests und 35 native Testprogramme; Hardware- und Safe-Builds einschließlich A/B. Der Kryptografie-Selbsttest wurde auf ESP8266 und ESP32 erfolgreich ausgeführt. Die noch offene Erstaufnahme-Abnahme bleibt oben ausdrücklich beschrieben.
