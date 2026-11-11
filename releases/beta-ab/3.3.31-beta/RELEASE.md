# LeafLink 3.3.31 Beta – Speicher beim Repeater-Update

Repeater reservieren beim Update nicht mehr den zusätzlichen RSA-Arbeitsbereich,
der für die laufende verschlüsselte Übertragung nicht gebraucht wird. Antworten
auf Datenblöcke verwenden nur 48 statt 560 Byte Arbeitspuffer. Der Flash-Schreiber
bleibt bei 1 KiB; seine bisherigen Speicherprüfungen bleiben erhalten.

Mit App 3.3.38 wird nach vollständigem Empfang zuerst die anstehende Prüfung
bestätigt. Anschließend gibt der Repeater seine Funk- und Empfangspuffer frei
und prüft Image, Hash und RSA-Signatur. Erst danach darf der inaktive Slot als
Startkandidat eingetragen werden. Die App meldet Erfolg erst nach passendem,
bestätigtem Neustart und dem Vergleich der Einstellungen und des Hausplans.

Zuerst App 3.3.38 installieren. Die Korrektur muss auf dem Repeater selbst laufen.
Wenn dessen bisherige Firmware schon beim Update-Start zu wenig Speicher hat,
ist einmalig ein Update im Routerbetrieb nötig; anschließend die Repeaterrolle
wiederherstellen. Dieses erste Update beweist den neuen Funk-Updateweg noch nicht.
Der reale Folgetest im Repeaterbetrieb wird nach dieser Erstinstallation geprüft.

Signiertes Hardware-Anwendungsupdate für ESP8266, 4 MiB, A/B-Layout 2.
Kopplungen, Räume, Einstellungen und Hausplan bleiben erhalten.
Die Gatewayübergabe und adaptive Gatewaywahl aus 3.3.30 sind enthalten.
