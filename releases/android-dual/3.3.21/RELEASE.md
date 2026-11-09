# LeafLink Android 3.3.21 – Innen- und Außentemperaturen je Lüfter

Die Lüftergruppenseite zeigt im Modus Sommerautomatik für jeden beteiligten Lüfter eine eigene Zeile mit **INNEN** und **AUSSEN**. Fehlende, ungültige oder veraltete Messungen erscheinen als Strich. Luftfeuchte und Bedienung bleiben verfügbar.

Hierfür alle beteiligten Lüfter auf **Firmware 3.3.19 Beta** aktualisieren. Sie enthält zugleich die Korrektur der Anmeldung bei fragmentiertem Gerätespeicher. Wall 0.6.6 Beta bleibt kompatibel.

Die App prüft die geräteeigene Temperaturantwort, Anfragekennung, Verbindung, Gruppe und Alter. Eine verlorene erlaubte Leseantwort wird begrenzt mit frischer Authentifizierung wiederholt. Eine vollständige Bedienbestätigung erfordert weiterhin die passenden Antworten aller angesprochenen Geräte.

Releasebuild, Lint, Protokoll-/Sicherheitstests und 24 Emulatorprüfungen der Sommerautomatik-Oberfläche bestanden. Die authentifizierten Temperaturabfragen wurden zusätzlich am echten Handy und Lüfter geprüft.

Signiertes Update für `de.prinz.leaflink`, Versionscode 30. Vorhandene App-Daten bleiben erhalten.
