# LeafLink 3.3.6 Beta – zuverlässiger Wechsel zwischen WLAN und Wall-Direktfunk

Gemeinsam mit Wall Control 0.6.2 verkürzt diese Version den Wechsel zwischen WLAN und Direktfunk. Gültige LAN-Antworten werden nicht mehr verworfen, wenn neuere Funkpakete vorher eintreffen. Authentifizierung, frische Sitzungsnachweise und Schutz vor wiederholten Paketen bleiben aktiv.

Auf zwei realen Lüftern wurden zwei vollständige Wechsel geprüft: jeweils etwa 18,5 Sekunden in den Direktfunk und 25,1 beziehungsweise 33,4 Sekunden zurück ins WLAN, statt zuvor über 100 Sekunden. Das sind Messwerte dieser Anlage, keine garantierten Höchstzeiten. Stufensteuerung, Sommer-/Wechselbetrieb, Nachtmodus und Ein/Aus wurden mit frischen Gerätebestätigungen geprüft.

Vorhandene Gruppen, Räume, Wall-Zuordnung, WLAN-Zugangsdaten und Einstellungen bleiben erhalten. Für die vollständige Korrektur auch die Wall auf 0.6.2 aktualisieren. Die Verbesserungen aus 3.3.4 für stabiles WLAN, geschützte Webbedienung und OTA sind enthalten.

In LeafLink unter Firmware-Updates die Beta-Versionen einschließen, Version prüfen und die Firmware aktualisieren. Die Android-App bleibt bei 3.3.4; ein App-Update allein installiert keine Lüfterfirmware.

Voraussetzungen: ESP8266 ESP-12F mit 4 MiB Flash, Hardwareprofil und bestehendem A/B-Layout 2. Nur die signierte firmware.bin über den regulären Updateweg verwenden. Kein Vollflash und kein Zurücksetzen. Für die geschützte Wall-Anbindung wird Wall 0.6.x benötigt; bei der Umstellung von Wall 0.5.x den Wall-Funknetzcode in der App übernehmen und die Lüfter mit physischer Freigabe koppeln. Bereits migrierte 0.6.x-Anlagen benötigen keine erneute Zuordnung.
