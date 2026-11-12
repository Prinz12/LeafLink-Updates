# LeafLink 3.3.32 Beta – Automatische Gegenrichtung bei Repeatern

Zwei Lüfter mit Installationsrichtung „Auto“ konnten im Repeaterbetrieb dieselbe
Grundrichtung wählen. Ihre Master-/Slave-Synchronisierung funktionierte, aber
die für die Richtungszuordnung benötigten Partnerdaten blieben auf den Gateways.

Gateways leiten bestätigte Statusdaten jetzt gezielt an Repeater derselben
Gruppe weiter. Das gilt für Partner am selben Gateway, an unterschiedlichen
Gateways und für Gateway-/Repeater-Paare. Die vorhandene Geräte-Reihenfolge
und der Vorrang einer manuell festgelegten Partnerrichtung bleiben erhalten.
Fremde Gruppen, eigene zurückgesendete Daten und Daten eines früheren Gateways
werden am Repeater abgewiesen. Die Weiterleitung verwendet vorhandene Puffer
und belegt keine zuverlässigen Steuerungs-/Update-Wiederholungsplätze.

Für die Korrektur beide Partner und alle möglichen Gateways auf 3.3.32 bringen.
Bei automatischem Gatewaywechsel empfiehlt sich derselbe Stand auf allen
Lüftern. „Auto“, Gruppen, Kopplungen, Hausplan und Einstellungen beibehalten.
App 3.3.38 kann weiterverwendet werden; kein neues App-Update erforderlich.
Die Speicherverbesserung für Repeater-Updates aus 3.3.31 ist enthalten.

Signiertes Hardware-Anwendungsupdate für ESP8266, 4 MiB, A/B-Layout 2.
Native Fehlerregression, Host-/Protokolltests, Hardwarebuild, Stackprüfung und
Android-Kompatibilitätsprüfungen bestanden. Die Gegenrichtung an den betroffenen
realen Lüftern muss nach Installation noch bestätigt werden.
