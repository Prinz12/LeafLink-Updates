# LeafLink 3.3.29 Beta – Signalqualität und Last bei der Gatewaywahl

Repeater berücksichtigen jetzt den WLAN-Empfang des Gateways, beobachtete
Beacon-Verluste, aktive Funkgeräte und belegte Sendewarteschlangen.
Eine bessere Route muss sich über mehrere Sekunden bewähren; gestaffelte
Haltezeiten und die vorausberechnete zusätzliche Last verhindern unnötige
gemeinsame Wechsel. Eine starre Gleichverteilung wird nicht erzwungen.
Unbekannte Messwerte gelten nicht als gute Verbindung. Mehrstufige Wege,
Controllerbindungen und automatische Ausfallübernahme bleiben erhalten.
Während des eigenen Firmwareuploads bleibt eine gesunde Route fest.

Die Funkqualität ist eine Zustellschätzung, kein ESP-NOW-RSSI; die Last ist
eine Schätzung aus Geräten und Warteschlangen, keine Bandbreitenmessung.
Für die vollständige Wirkung alle beteiligten Gateways und Repeater aktualisieren.

Enthält außerdem die Korrekturen gegen Gateway-Speichermangel, bestätigte
Identitätsanfragen und eine Funkbestätigung erst nach tatsächlicher Aufnahme
in die Anwendung. Abgewiesene Nachrichten können dadurch erneut zugestellt werden.
Für die Hintergrundsuche in der App wird Android 3.3.36 empfohlen.

Signiertes Hardware-Anwendungsupdate für ESP8266, 4 MiB, A/B-Layout 2.
Bestehende Einstellungen, Räume, Kopplungen und Hausplan bleiben erhalten.
