# LeafLink 3.3.53 – Sparsamere Netzprüfung

Die Netzwerkansicht liest mit Firmware 3.3.50 nur die benötigten Netzwerkdaten
und lädt die gemeinsame Geräteliste einmal je Aktualisierung. Das reduziert
HTTP-Daten und Arbeit auf den Lüftern deutlich.

Ältere Firmware bleibt unterstützt. Nur ein fehlender neuer Endpunkt erlaubt
den bisherigen vollständigen Statusabruf; Überlast und Verbindungsfehler lösen
keine zusätzliche große Abfrage aus. Geräteidentitäten werden weiterhin geprüft.

Die sichere Auswahl des Updatewegs aus App 3.3.52 bleibt enthalten.
Bestehende Kopplungen, Hausplan und App-Einstellungen bleiben erhalten.

Die echte Netzansicht wurde auf dem angeschlossenen Tablet in sieben
Durchläufen geprüft; zusätzlich bestanden Hosttests, Build, Lint und
Emulatorprüfungen zu Darstellung, Identität, Fehlerfällen und Updateweg.
