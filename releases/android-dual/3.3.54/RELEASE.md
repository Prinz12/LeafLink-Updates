# LeafLink 3.3.54 – Firmware-Uploads über VPN

Behebt einen vorzeitigen Zeitabbruch beim direkten Firmware-Upload:
Die App wartet innerhalb des bestehenden Gesamtlimits von sechs Minuten auf
die Geräteantwort. Das bisherige zusätzliche Limit von 45 Sekunden konnte
Updates über langsamere Verbindungen abbrechen, obwohl noch Daten übertragen
oder auf dem Lüfter geprüft wurden.

Die Fortschrittsanzeige bleibt bis zur erfolgreichen Geräteantwort bei
höchstens 99 Prozent. Anschließend werden Neustart, Firmware und gespeicherte
Einstellungen weiterhin separat geprüft. Der Updatehinweis nennt jetzt
ausdrücklich WLAN oder VPN.

Keine automatische Wiederholung unklarer Uploads. Bestehende Kopplungen,
Hausplan und Einstellungen bleiben erhalten. Keine neue Lüfterfirmware nötig.

Nach dem App-Update einen abgebrochenen Versuch über „FEHLVERSUCH PRÜFEN“
prüfen lassen und anschließend erneut starten.
